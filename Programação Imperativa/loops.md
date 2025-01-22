# Loops

Loops (ou repetições) são estruturas que, dada uma uma condição, ele testa uma condição, e enquanto ela for verdadeira, um determinado bloco de código será repetido.

## while

O ```while``` é uma estrutura que testa uma condição ao início da execução de um bloco de código, e se ela for verdadeira, ele será executado. Ao fim de cada execução, essa condição será testada. Se, em determinada execução, esta condição não for satisfeita, o bloco de código deixa  de ser executado.

```c
int x = 1;

while (x < 10){
  printf("%d",x);
  x++;
}
```
O código acima executa a impressão do número da variável x, e acresce 1 a essa variável, enquanto x é menor que 10.

Similar ao conceito de recursividade, aqui, temos um caso base (x menor que 10) e um passo indutivo (x++), além dos comandos envolvidos.

##while do

##for
