# Estruturas de decisão múltipla

Além das estruturas de decisão ```if ``` e ```else```, existe a estrutura de decisão múltipla ```switch```:
```c
switch(variável){
    case constante1:
        comando;
        break;
    case constante2:
        comando;
        break;
    default:
        comando;
}
```

A palavra ```switch``` é acompanhada de uma variável discreta (char ou int e derivados), a qual a condição será testada. O uso da palavra ```case``` determina os casos a serem testados, isto é, os casos em que o valor da variável corresponde ao valor desejado.

A palavra ```default``` representa o conjunto de ações que será executado caso nenhuma das condições testadas seja satisfeita. Seu uso é opcional.

OBS¹: Para executar apenas o primeiro ```case``` correspondente a um valor, é necessário utilizar a palavra reservada ```break```

OBS²: O ```switch``` não aceita strings ou floats. Para testar condições com variáveis desses tipos, é necessário utilizar ```ìf``` e ```else```.