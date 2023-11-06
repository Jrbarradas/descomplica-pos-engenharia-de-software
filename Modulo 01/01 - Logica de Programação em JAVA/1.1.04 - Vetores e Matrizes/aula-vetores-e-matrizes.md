# Vetores e Matrizes

# Exercícios


## Questão 01
Observe com atenção o código a seguir:

| 1    | int[] lista = {3,4,5,6,7};       |
| ---- | -------------------------------- |
| 2    |                                  |
| 3    | int cont = 0;                    |
| 4    |                                  |
| 5    | while(cont < 5){                 |
| 6    | System.out.println(lista[cont]); |
| 7    | cont = cont + 1;                 |
| 8    | }                                |
| 9    | for(cont=0; cont<5; cont++)      |
| 10   | System.out.println(lista[cont]); |

Considerando essas informações e os conteúdos estudados sobre estrutura de repetição, analise as asserções a seguir e a relação proposta entre elas.

I. No laço da linha 5, o nosso programa tem um while cuja execução (iteratividade) será encerrada assim que a variável cont atingir o valor 5, mostrando os 5 valores da lista.

Porque:

II. Todo laço de repetição necessita de uma condição de parada definida somente na condição do while ou na do for. Neste exemplo, se no laço while a condição de parada está na linha 5, no segundo laço temos a condição de parada na linha 9, e é cont < 5.

A seguir, assinale a alternativa correta.

### Resposta:

- a) ​A asserção I é uma proposição verdadeira, e a II é uma proposição falsa

> SOLUÇÃO DO PROFESSOR ✨
>
> A proposição I está correta, pois a condição de parada deste algoritmo será quando o valor da variável cont for igual a 5. Deste modo, temos incremento na variável cont, e a parada será realizada assim que a condição dentro do while for falsa. A proposição II está incorreta, pois, apesar de praticamente todo laço de repetição possuir uma condição de parada, nem todo laço precisa ter uma. Por exemplo:
>
> • Looping para execução contínua: Em sistemas embarcados ou em tempo real, pode haver situações em que um programa precisa executar continuamente sem parar até que ocorra algum evento externo ou que o próprio sistema seja desligado. Nestes casos, o programa pode ser projetado para executar um loop infinito sem uma condição de parada explícita.
>
> • Looping de tarefas de monitoramento: Em alguns sistemas de monitoramento ou controle, pode ser necessário que uma tarefa específica seja executada repetidamente para verificar o estado de algum processo ou variável em tempo real. Nesses cenários, a condição de parada pode ser substituída por uma verificação do status do processo ou variável, decidindo se o loop deve continuar ou não.
>
> No entanto, é importante projetar esses loopings cuidadosamente para evitar possíveis problemas. Em loops sem uma condição de parada explícita, é fundamental garantir que haja uma maneira externa de interrompê-los quando necessário, como um evento de desligamento do sistema ou a mudança de uma variável específica.
>
> Em resumo, embora existam situações em que um looping de programação não tenha uma condição de parada explícita, é uma prática comum e geralmente mais segura incluir uma condição de parada adequada para garantir o bom funcionamento do programa e evitar loops infinitos indesejados.


## Questão 02
Observe com atenção o seguinte código escrito em Java.

int[] valores = {9,8,7,6,5};
int aux;
int cont = 0;
while (cont < 2){
aux = valores[cont];
valores[cont] = valores[cont+1];
valores[cont+1] = aux;
cont += 1;

}

for (int i=0; i<5; i++){
System.out.println(valores[i]);

}

### Resposta:
- a) Na linha 12, a lista estará com esta sequência de valores 8 7 9 6 5

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra A, pois o código tem como objetivo trocar alguns valores dentro da lista. Utilizamos a estrutura de repetição while para percorrermos a lista. Na primeira iteração, ao entrar no while, o valor de cont é zero. Nós então estamos pegando o valor na posição zero da lista e guardando na variável aux, que serve como memória temporária. Em seguida, pegamos o valor na posição cont + 1, ou seja, na posição 1 da lista e colocamos na posição zero da lista. Por fim, guardamos o valor que estava na variável aux para dentro da lista na posição 1. Note, por 2 vezes nós realizaremos as trocas seguindo esta ordem que foi exposta. Deste modo, ao final da execução teremos duas trocas, na primeira troca a lista fica assim: 8 9 7 6 5 e na segunda troca ele fica assim: 8 7 9 6 5, que é a solução da questão. Se houvesse mais uma troca, a lista ficaria assim: 8 7 6 9 5.


## Questão 03
Considere um analista que, baseado em uma lista com 10 valores numéricos inteiros, deseja analisar quantos destes são pares e quantos são maiores que 28. Para isso, ele criou o seguinte algoritmo.

| 1    | int[] lista = {13,41,5,86,72,9,82,36,27,8};           |
| ---- | ----------------------------------------------------- |
| 2    |                                                       |
| 3    | int pares = 0;                                        |
| 4    | int maiores = 0;                                      |
| 5    |                                                       |
| 6    | ?                                                     |
| 7    | ?                                                     |
| 8    | pares = pares + 1;                                    |
| 9    | if(lista[i] > 28)                                     |
| 10   | maiores = maiores + 1;                                |
| 11   |                                                       |
| 12   | System.out.println(“Pares são: “ + pares);            |
| 13   | System.out.println(“Maiores que 28 são: “ + maiores); |

A única dúvida do analista é o que colocar nas linhas 6 e 7. Considerando as informações apresentadas, assinale a opção que, corretamente, pode ser inserida respectivamente nas linhas 6 e 7.

### Resposta:

- c) Linha 6: for (int i=0; i <10; i++) e linha 7: if (lista[i] % 2 == 0)

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra C, pois na linha 6 é necessário colocar uma estrutura de repetição para percorrer a lista apresentada. Temos duas opções, utilizar o while ou utilizar o for. Como não podemos acrescentar conteúdo em outras linhas a não ser nas linhas com a interrogação, então, nos resta utilizar o laço for, o qual será definido com a seguinte estrutura for (int i=0; i <10; i++). Em seguida, temos que fazer uma validação se o valor obtido da lista é par, para isso, utilizaremos o módulo. Todo número é considerado par se, ao dividi-lo por 2 o resto for igual a zero, logo, a estrutura do if será if (valor % 2 == 0).


## Questão 04
Considere o código a seguir onde temos um vetor e uma estrutura de repetição o percorrendo.

| 1    | int[] lista = {8,1,3,5,16,7,9,41,2,10}; |
| ---- | --------------------------------------- |
| 2    |                                         |
| 3    | int x = lista[0];                       |
| 4    |                                         |
| 5    | for(int i=0; i<10;i++)                  |
| 6    | if(lista[i] % 2 == 0)                   |
| 7    | if(lista[i] > x)                        |
| 8    | x = lista[i];                           |
| 9    |                                         |
| 10   | System.out.println(“Resultado: “ + x);  |

Considerando as informações apresentadas neste código-fonte, avalie as afirmações a seguir:

 I. O laço for percorrerá toda lista a procura de um valor par, armazena este valor na variável x e o apresenta na linha 10.

II. O laço for percorrerá toda lista a procura do maior valor par, o armazena na variável x e apresenta o seu valor na linha 10.

III. A variável x receberá um valor da lista na linha 3 e, na linha 7, o valor da variável x é comparado com um valor da lista.

IV. As linhas 6 e 7 podem ser colocadas em uma única instrução if(lista[i] % 2 == 0 || lista[i] > x), e a saída será a mesma.

 Estão corretas apenas as afirmativas:

### Resposta:

- b) II e III, apenas

> SOLUÇÃO DO PROFESSOR ✨
>
> A afirmativa II está correta, pois na linha 3 a variável x recebe o primeiro valor da lista. Em seguida, na linha 5 temos um laço for que percorre toda a lista. Na linha 6 fazemos um teste, valor a valor para verificar se o número é par. Se o número for par, então verificamos se ele é maior que o primeiro valor da lista, se for maior, então atribuímos este novo valor a x, deste modo, o objetivo é encontrar o maior valor par da lista.
> A afirmativa III está correta, pois a variável x recebe o primeiro valor da lista e, na linha 7, este valor será comparado com todos os valores da lista, até chegar ao final dela.

