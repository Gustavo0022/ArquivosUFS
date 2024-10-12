# Recursividade

## Conceito

Recursividade é o ato de resolver um problema por meio da repetição de uma mesma função, chamada de **passo indutivo**, invocada por ela mesma, até que se chegue ao chamado **caso base**

O **CASO BASE** é o valor inicial de uma sequência recursiva. Ele é responsável por definir o fim da cadeia recursiva.

Já o **PASSO INDUTIVO** é o passo necessário para transitar até o caso base, assim obtendo o resultado esperado.

Ex.: Definindo uma sequência aritmética $ \{3,5,7,9,11,13...\}$, podemos obter qualquer valor dela por meio da função recursiva a seguir

>$f(0) = 3 $  
$ f(n-1) + 2$  

A primeira linha é o Caso Base (que indica que $3$ é o elemento inicial da sequência e que, se o "contador" chegar a 0, o valor será $3$ ) e a segunda é o passo indutivo (que indica que, enquanto $f(n)$ for diferente de zero, subtri-se o n em 1 e soma-se 2 ao resultado de $f(n-1)$ ). Assim, para chegar ao quarto elemento da sequência, seriam feitos a seguintes iterações:

"Ida" até o caso base

>$f(3)$ =  
=$f(2) + 2$  
=$f(1) + 2$  
=$f(0)$ → 3

"Volta" solucionando os passos indutivos recursivamente

>$f(1) + 2$ → $3 + 2 $ = 5  
$f(2) + 2$ → $5 + 2$ = 7  
$f(3) + 2$ → $7 + 2$ = 9

Logo, o quarto elemento da lista é $9$

Outro exemplo de função recursiva é a famosa **Sequência de Fibbonacci**, que pode ser representada da seguinte forma:

>$f(0) = 1$       (caso base 1)  
$f(1) = 1$        (caso base 2)  
$f(n-1) + f(n-2)$ (passo indutivo)

Traduzindo em palavras, os casos base são os primeiros números da sequência $(1,1)$ e todos os outros derivam desses, nesse caso, o elemento $f(3)$ é definido por $f(2) + f(1)$, ou melhor, $3 = 2+1$

Na programação, utilizando JavaScript essa função pode ser representada por:

```js
const fib = (n) => {
    if (n == 0) return 1
    else if (n == 1) return 1
    else return fib(n - 1) + fib(n-2)
}
```

Note que a função é chamada dentro dela mesma, e isso é um dos aspectos que caracteriza uma função recursiva. Note também que, caso não existissem casos base, a função nunca terminaria de ser executada, resultando em uma "stack overflow" ou sobrecarga de pilha.

