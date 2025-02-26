# Funções

Apesar de já usarmos funções desde quando começamos a programar, é possível também criarmos nossas próximas funções.

É altamente recomendado criar funções para códigos que se repetem.

É uma boa pŕatica que funções realizem uma única tarefa, e seu nome reflita essa tarefa.


## Definição e chamada de uma função

Funções podem ser definidas com a seguinte sintaxe

```c
void soma(int x, int y){ //<- Declaração da função com os argumentos a serem manipulados
  int valorSoma;
  valorSoma = x+y;
  printf("%d", valorSoma);
}

int main(){
  soma(3,2); //<- Chamada da função com os parâmetros passados
}
```

A sintaxe de definição de funções deve ter, obrigatoriamente, o tipo do retorno, o nome da função e a lista de parâmetros necessários para executá-la.
Quando a função não necessida de parâmetros, os parênteses ainda são utilizados (a exemplo da função main).

**OBS:** Cada argumento requisitado por uma função deve conter, em sua definição, o tipo da variável a ser recebida. Ex: ```int troca(int x, int y){...}```. Note que, mesmo com os argumentos sendo do mesmo tipo (int), a palavra reservada para esse tipo é utilizada para cada argumento. Caso a função fosse definida como ```int troca(int x, y){...}```, o código não funcionaria.

Variáveis declaradas dentro de funções de forma estática possuem tempo de vida limitado até o fim da execução da função e escopo limitado, não existindo fora da função.


Para chamar uma função, é necessário utilizar o nome desta, junto aos argumentos esperados por ela (definidos quando a função foi definida).



## Passagem de argumentos para funções

Argumentos podem ser passados por valor ou por referência.

Ao passar um argumento por valor,

Ao passar um argumento por referência,
