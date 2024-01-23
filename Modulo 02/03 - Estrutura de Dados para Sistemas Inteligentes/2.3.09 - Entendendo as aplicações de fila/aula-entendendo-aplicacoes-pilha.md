# Entendendo as Aplicações de Fila

# Exercícios


## Questão 01
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Fila a que o algoritmo se refere:

Enfileirar (elemento numérico_inteiro)

 início_módulo

  se (não FilaCheia( ))

   então

​    vetor[fim] ← elemento;

​    fim ← fim + 1;

​    total ← total + 1;

​    se (fim > = tamanho)

​     então

​      fim ← 0;

​    fimse;

   senão

​    escrever ("Fila Cheia");

  fimse;

 fim_módulo;

### Resposta:
- a) insere um elemento no final da fila

> SOLUÇÃO DO PROFESSOR ✨
>
> Enfileirar é uma operação de manipulação da Fila que insere um elemento no final da fila, o acesso é no final da fila


## Questão 02
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Fila a que o algoritmo se refere:

numérico_inteiro Desenfileirar ()

 início_módulo

  Declarar

   desenfileirado ← 0 numérico_inteiro;

 

  se (FilaVazia()) então

​    escrever ("Fila Vazia");

   senão

​    desenfileirado ← vetor[inicio];

​    inicio ← inicio + 1;

​    total ← total – 1;

​    se (inicio >= tamanho) então

​      inicio ← 0;

  fimse;

  retornar desenfileirado;

 fim_módulo;

### Resposta:
- b) remove um elemento do início da fila

> SOLUÇÃO DO PROFESSOR ✨
>
> Desenfileirar é uma operação de manipulação da Fila que remove um elemento do início da fila, o acesso se dá pelo início da Fila


## Questão 03
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Fila a que o algoritmo se refere:

lógico FilaVazia( )

 início_módulo

  se (total = 0)

   então

​    retornar verdadeiro;

  senão

   retornar falso;

  fimse;

 fim_módulo;

### Resposta:
- c) verifica se a fila está vazia

> SOLUÇÃO DO PROFESSOR ✨
>
> Fila Vazia é uma operação de manipulação da Fila que verifica se a fila está vazia, a verificação acontece pelo total de elementos da Fila


## Questão 04
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Fila a que o algoritmo se refere:

lógico FilaCheia( )

 início_módulo

  se (total >= tamanho)

   então

​    retornar verdadeiro;

   senão

​    retornar falso;

  fimse;

 fim_módulo;

### Resposta:
- d) verifica se a fila está cheia

> SOLUÇÃO DO PROFESSOR ✨
>
> Fila Cheia é uma operação de manipulação da Fila que verifica se a fila está cheia. O acesso se dá pelo total de elementos da Fila

