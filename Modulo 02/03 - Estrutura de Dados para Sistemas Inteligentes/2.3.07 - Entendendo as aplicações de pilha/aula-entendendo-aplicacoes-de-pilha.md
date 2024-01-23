# Entendendo as Aplicações de Pilha

# Exercícios


## Questão 01
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Pilha e a qual algoritmo se refere:

Empilhar (elemento numérico_inteiro)

 início_módulo

  se (não PilhaCheia( ))

   então

​    topo ← topo + 1;

​    vetor[topo] ← elemento;

   senão

​    escrever ("Pilha Cheia");

  fimse;

 fim_módulo;

### Resposta:
- a) insere um elemento na pilha

> SOLUÇÃO DO PROFESSOR ✨
>
> Empilhar é uma operação de manipulação de Pilha que insere um elemento na Pilha. A inserção ocorre no topo da Pilha


## Questão 02
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Pilha e a qual algoritmo se refere:

inteiro Desempilhar ()

 início_módulo

  Declarar

   desempilhado ← 0 numérico_inteiro;

 

  se (PilhaVazia())

   então

​    escrever ("Pilha Vazia");

   senão

​    desempilhado ← vetor[topo];

​    topo ← topo – 1;

  fimse;

  retornar desempilhado;

 fim_módulo**;**

### Resposta:
- b) remove um elemento da pilha

> SOLUÇÃO DO PROFESSOR ✨
>
> Desempilhar é uma operação de manipulação da Pilha que remove um elemento da Pilha. A remoção ocorre pelo topo da Pilha


## Questão 03
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Pilha e a qual algoritmo se refere:

lógico PilhaVazia( )

 início_módulo

  se (topo = – 1)

   então

​    retornar verdadeiro;

  senão

   retornar falso;

  fimse;

 fim_módulo;

### Resposta:
- c) verifica se a pilha está vazia

> SOLUÇÃO DO PROFESSOR ✨
>
> Pilha Vazia é uma operação de manipulação da Pilha que verifica se a pilha está vazia. A verificação ocorre pela variável topo


## Questão 04
Observe o algoritmo abaixo e indique qual é a operação de manipulação da Pilha e a qual algoritmo se refere:

lógico PilhaCheia( )

 início_módulo

  se (topo >= tamanho – 1)

   então

​    retornar verdadeiro;

   senão

​    retornar falso;

  fimse;

 fim_módulo;

### Resposta:
- d) verifica se a pilha está cheia

> SOLUÇÃO DO PROFESSOR ✨
>
> Pilha Cheia é uma operação de manipulação da Pilha que verifica se a pilha está cheia. A verificação ocorre pela variável topo

