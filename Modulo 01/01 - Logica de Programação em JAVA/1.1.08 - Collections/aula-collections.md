# Collections

# Exercícios


## Questão 01
Considere o exemplo de um cofrinho. Todos nós o tivemos durante a nossa infância, onde costumávamos guardar nossas moedas. Este cofrinho chama-se Coleção e as moedas não passam de objetos. Tecnicamente, uma coleção é um objeto ou um contêiner que armazena um grupo de outros objetos.
Considere então as afirmativas a seguir

I. o framework Java Collection é uma arquitetura para manipular e representar coleções em Java

II. o framework Java Collection é uma hierarquia formada por interfaces e classes

III. o framework Java Collection necessita que o desenvolvedor implemente a arquitetura de interfaces e classes

Está correto apenas o que se afirma em:

### Resposta:
- a) I e II, apenas

> SOLUÇÃO DO PROFESSOR ✨
>
> A afirmativa I está correta, pois o Collections Framework é definido como uma arquitetura unificada para representar e manipular coleções. A afirmativa II está correta, pois o Collections Framework é uma hierarquia de interfaces e classes que facilita o gerenciamento de um grupo de objetos. A afirmativa III está incorreta, pois o framework fornece uma arquitetura pronta para interfaces e classes e usada para armazenar e manipular um grupo de objetos


## Questão 02
Antes do lançamento do framework Java Collection, Vectores, Stacks e Arrays estavam lá e eram muito utilizados. A grande desvantagem é que eles não tinham uma interface comum e interconexão entre si. Nesse caso, torna-se tedioso para o usuário lembrar de todas as funções e sintaxe. Além disso, as formas convencionais, como arrays e pilhas, não estavam fornecendo o desempenho e a flexibilidade desejados.
Dentre as diversas implementações, a interface List é implementada por quais classes?

### Resposta:
- e) LinkedList, ArrayList, Vectors e Stack

> SOLUÇÃO DO PROFESSOR ✨
>
> A interface List é implementada pelas classes LinkedList, ArrayList, Vectors e Stack


## Questão 03
O framework Java Collections fornece alto desempenho e alta eficiência. Isso se deve ao fato de que várias implementações de cada interface são intercambiáveis, de modo que os programas podem ser escritos por implementações de comutação. Alguns métodos de cada interface do Collections Framework possuem uma implementação uniforme. A API Collections possui interfaces básicas como Set, Map e List, então as classes que as implementam possuem alguns conjuntos comuns de métodos.
De posse desta informação, marque a alternativa que apresenta métodos responsáveis por adicionar, remover e verificar se um objeto está presente na coleção

### Resposta:
- b) add(obj), clear(), contains(obj)

> SOLUÇÃO DO PROFESSOR ✨
>
> add() é usado para adicionar um objeto à coleção, clear() é responsável por remover todos os elementos da coleção e contains() verifica se o objeto está presente na coleção e retorna true se encontrado


## Questão 04
Considere um ArrayList de números inteiros do código a seguir

| 1    | ArrayList<Integer> lista = new ArrayList<>(); |
| ---- | --------------------------------------------- |
| 2    | for(int i=0; i<8; i++)                        |
| 3    | lista.add(i, i+1);                            |
| 4    | System.out.println(lista.get(4));             |

 

Sobre a execução e saída deste código, marque a alternativa correta.

### Resposta:
- d) Este código retornará o valor que está no índice 4 da lista, que neste caso, é o número 5

> SOLUÇÃO DO PROFESSOR ✨
>
> O método get recebe como parâmetro o atributo de índice e, como consequência, retornará o valor presente no índice indicado que, neste caso, é o índice 4, o qual retornará o valor 5

