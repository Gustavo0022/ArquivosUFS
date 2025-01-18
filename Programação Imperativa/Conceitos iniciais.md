# Conceitos Iniciais - Programação Imperativa


## Programa e algoritmo

Algoritmos são sequências de passos a serem executados. Esses passos são bem descritos, sem ambiguidades, e que podem ser executados de alguma forma. Por exemplo, para calcular a soma de dois números, você toma esses dois número, processa-os de forma a somá-los, e retoma o resultado dessa soma.

Um programa é uma sequência de passos escrita em uma linguagem de computador para executar ações ou resolver problemas. Eles são essenciais para o funcionamento de um computador, afinal sem programas, a máquina é inútil. Seu Sistema Operacional(Windows,Linux, Mac OS ou BSD) são programas; seu aplicativo de calculadora é um programa; o navegador pelo qual você provavelmente lê isso é um programa. 

Para a criação de programas, é necessária alguma interface entre o programador e o computador. Monitores, terminais de computador, ou impressoras para ver os comandos digitados e os resultados; dispositivos para a entrada de dados (um teclado, por exemplo); e algo que seja possível escrever esses programas de forma que o computador entenda. É aí que entram as linguagens de programação.

O computador só entende instruções em binário, isto é, 0 e 1, sim ou não. É com sequências de zeros e uns que os programas rodam no computador. Mas escrever em binário (também chamado de linguagem de máquina) é trabalhoso e difícil. Por isso, foram inventadas diferentes linguagens de programação, como assembly, que, mesmo sendo mais fácil que linguagem de máquina, ainda é complicado para padrões atuais. Então, ao longo do tempo, diferentes linguagens foram construídas de forma a facilitar ainda mais a construção e a criação de programas, como COBOL, Fortran, Lisp, C, Java, entre outras. Aqui, daremos enfoque na linguagem C.


## Trinômio

Para o funcionamento do programa, é necessário entender o objetivo desse programa, e assim entender:

* A entrada: Os dados inseridos para cumprir o objetivo
* O processamento: A manipulação dos dados para obter o resultado desejado
* A saída: O resultado do algoritmo

## A linguagem C

C foi criada nos Laboratórios Bell (AT&T) por Denis Ritchie e Ken Thompson em 1970. É uma linguagem de alto nível, mesmo que considerada por alguns como de nível médio devido ao acesso de memória. É compilada, estruturada e fortemente tipada.

Ser uma linguagem compilada significa que o código do programa é convertido para linguagem de máquina por inteiro. Isso é diferente de linguagens interpretadas,como python, que lê o código e o converte linha a linha.

## Termos

* Código fonte: é o código do 
* Código objeto:
* Linkeditor:
* Código executável:
* Biblioteca:
* Tempo de compilação:
* Tempo de execução (runtime):


## Exemplo de programa em C

```c
#include <stdio.h> /*Biblioteca*/

int main(){ //função main
    printf("Hello world!");
}
```

O ```include <stdio.h>``` significa que a biblioteca stdio.h (standard Input/Output) é requisitada para a execução do programa. Essa biblioteca é a principal biblioteca da linguagem, pois contém todas as funções básicas.

A função ```main()``` é a principal função do C. Ela executa as funções subsequentes necessárias para executar o programa.

## Variáveis

Variáveis são dados guardados de forma provisória na memória RAM da máquina. Cada um desses dados é endereçado.

As variáveis podem ocupar diferentes quantidades de memória. Ex.: Um caractere ocupa 1 byte, enquanto um número inteiro (int) ocupa 4 bytes.

No caso da linguagem C, as regras de nomenclatura são:

* O primeiro caractere pode ser uma letra ou _(underline)
* Caracteres maiúsculos e minúsculos são diferentenciados (Case sensitive)
* As variáveis não podem ser iguais a palavras reservadas da linguagem
* Os nomes das variáveis não podem possuir espaços em branco

As variáveis podem ser:
* Locais (declaradas dentro de funções)
* Na definição de parãmetros de função
* Fora de todas as funções (variáveis globais)
* 

### Tipos de variáveis

Como indicado antes, as variáveis podem ocupar diferentes quantidades de memória a depender do tipo. Os tipos de variáveis podem ser usados para determinar a quantidade de memória ocupada e para determinar se é possível realizar operações com outras variáveis. (Ex.: uma variável de tipo int não pode realizar operações com uma variável do tipo char)


Os tipos de variáveis em C são:
* Int: número inteiro (16 bits)
* float: números racionais (32 bits)
* double: números racionais (64 bits)
* long int: número nteiro (32 bits)
* char: valores alfanuméricos (1byte)
* void: valor ...


## Comentários em C

Os comentários em C são feitos com ```/* comentário */```

## Operadores aritméticos

Os operadores aritméticos em C são
* -:
* +:
* *:

## Máscaras de formatação de E/S

* %d: Int
* %f: Float
* %c: Char
* %s: String

Essas máscaras são usadas para capturar ou exibir dados de variáveis. Ex.:

```c
int numero = 3;
printf("%d", numero);
```

## Entrada e Saída

A entrada de dados se dá da seguinte forma:
```c
int numero;
scanf("%d", &numero);
```

O ```&``` é o operador de endereçamento de valores na memória. 

Já a saída se dá da seguinte forma

```c
int numero = 3;
printf("%d", número)
```


## (Programa) Cálculo de média aritmética da nota de dois alunos

```c
#include <stdio.h>

float nota1,nota2,media;

void main(){

    printf("Insira a primeira nota: ");
    scanf("%f", &nota1);
    printf("\n Insira a segunda nota: ");
    scanf("%f",&nota2);

    media = (nota1 + nota2)/2;

    printf("\n A média das notas é %f",media);
}

```

