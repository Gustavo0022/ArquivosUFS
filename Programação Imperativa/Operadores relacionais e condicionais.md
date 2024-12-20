# Operadores relacionais e estruturas condicionais

## Operadores relcaionais

A linguagem C possui operadores chamados, operadores relacionais, que servem para comparar dados (variáveis, inteiros, strings, etc.).

Alguns operadores relcaionais são:

* < (Menor que)
* \> (Maior que)
* <= (Menor ou igual)
* \>= (Maior ou igual)
* == (igual)
* != (diferente de)

Baseado nisso, podemos realizar operações de comparação em chamadas **estruturas de decisão**.

## Estruturas de decisão simples

As estruturas de decisão simples interrompem o fluxo de tempo de execução do programa a depender dos valores passados. Elas são representadas pelas palavras ```if``

```C
...
if ("condição"){
    print("condição satisfeita");
}
...
```

No código acima, a palavra "condição" pode ser substituida por alguma comparação, e caso satisfeita, ela executará o código determinado, nesse caso ```print("Condição satisfeita");```. Veja o exemplo abaixo

```c
   int x, y, z;
    printf("Bem vindo");
    printf("\nInsira o primeiro valor:");
    scanf("%i", &x);
    printf("\nInsira o segundo valor:");
    scanf("%i", &y);

    z = x+y;

    if(z > 10){
        printf("A soma dos dois  números é %i",z);
    }
```

O código acima recebe dois números digitados pelo usuário, e os soma. Caso a soma desses números seja superior a 10, ele exibe o resultado.

## Estruturas de decisão compostas

Em comparação com as estruturas de decisão simples, aqui, possuímos a condicional ```else```
