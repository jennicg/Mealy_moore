# Mealy_moore
Autores: <br>
Jennifer de Castro: jenny_cg23@hotmail.com<br>
Larissa Motta: larissasantosdamotta@gmail.com <br>
<br>
<br>
<b>TUTORIAL </b>

O programa foi desenvolvido em python. A explicação do código foi feita em comentários no próprio programa. 
 Para o desenvolvimento deste trabalho era necessário utilizar SExpression, o qual foi utilizado um código obtido através do site: http://rosettacode.org/wiki/S-Expressions#Python Para realizar sua execução basta apenas ir no prompt de comando e digitar o nome do programa, que no caso é main.py, o nome do arquivo de entrada e o nome do arquivo de saída. Segue em anexo um exemplo:

python3 main.py  mealy-to-moore1.txt  maquinaSaida.txt

![](https://github.com/jennicg/Mealy_moore/blob/master/LFAEXEMPLO.png)


DESCRIÇÃO BREVE DA ESTRUTURA DO CÓDIGO

Na conversão de maquina de moore para mealy percorre-se as transições, onde são feitas algumas validações para verificar se a entrada passada como parametro atende aos requisitos e tambem a reconfiguração das transições e a adição dos out-fn.

A conversão de mealy para moore, comparado a conversão citada anteriormente, é bem mais complexa. É criado um dicionario com os estados, depois disso é percorrido as transições onde é feita algumas validacoes e  é adicionado ao dicionario suas saidas.
Ao percorrer esse dicionario obtem-se novos estados, caso necessário. Para obter as novas transições é necessário passar novamente pelas transições da mealy. Por fim verifica-se os estados finais.
