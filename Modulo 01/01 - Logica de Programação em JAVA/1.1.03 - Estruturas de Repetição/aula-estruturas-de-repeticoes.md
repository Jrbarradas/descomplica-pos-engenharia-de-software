# Estruturas de Repetições

# Exercícios


## Questão 01
Observe com atenção o código a seguir:

for(int x=1; x<10; x++)

   if(x%4 !=0 && x%2 ==0)

​    for(int y=1; y<5; y++)

​     System.out.println(y);

Neste código temos duas estruturas de repetição for aninhadas, sendo que o for interno está dentro de uma estrutura condicional. Considerando as informações apresentadas neste código, assinale a opção correta.

### Resposta:
- a) A linha 4 será executada em um total de 8 vezes, apresentando a sequência 12341234
-  

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra A, pois o for externo executará 9 vezes (de 1 a 9, exceto o 10) o bloco que se inicia na linha 2. Como a única condição para entrar no bloco if da linha 2 é que o valor de x não seja divisível por 4 E o valor de x seja par (ou divisível por 2), então a linha 4 será executada 8 vezes apresentando os valores 12341234.


## Questão 02
Observe com atenção o seguinte código escrito em Java

 int d, x;

  d = 0;

  x = 314;

  while (x>1){

   x = x/2; d = d+1;

  }

  System.out.println(x);

  System.out.println(d);

Considerando o uso de uma estrutura de repetição na linha 3 deste código, marque a alternativa que apresenta respectivamente os valores de x e d após a execução do laço while. 

### Resposta:
- c) x = 1; d = 8.

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra C, pois a variável que controla a estrutura de repetição é o x. Observe que na primeira execução, o valor de x é 314. Como este valor é maior que 1, então o laço while é executado. Em seguida, na linha 5, estamos realizando duas operações. Primeiramente dividindo o valor de x por 2 e armazenando o resultado na variável x; em segundo lugar estamos somando 1 na variável d e, em seguida, armazenando na própria variável d. Observe que esta operação é feita várias vezes, até que o valor de x (que está sendo dividido) seja menor que 1, então, o laço de repetição é interrompido. Logo, o valor da variável x será 1 e o valor da variável d será 8, que é o número de vezes que o laço while será executado.


## Questão 03
Observe com atenção o código a seguir, onde temos uma variável n que não possui valor declarado, porém, aceita qualquer valor inteiro positivo ou negativo. 

| 1    | int n;                         |
| ---- | ------------------------------ |
| 2    | int cont =0;                   |
| 3    | for(int i=1; i<(n+1); i++)     |
| 4    | if(n%i == 0)                   |
| 5    | cont = cont + 1;               |
| 6    | System.out.println(cont == 2); |

### Resposta:
- d) n for um número primo

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra D. Vamos antes relembrar que número primo é aquele que é divisível por 1 e por ele mesmo, ou seja, um número primo possui apenas 2 divisores. Agora vamos ao código. Temos uma variável chamada cont, a qual contabilizará quantas vezes o número n é divisível por um valor do intervalo de 1 a n+1. Logo, se cont for igual a 2, ou seja, se houve apenas 2 divisões exatas, com resto igual a zero, então retornará true, caso contrário, retornará zero. Por exemplo, se o valor de n for igual a 4, então teremos 4/1 terá resto da divisão igual a zero, então cont passa para 1, em seguida, 4/2 terá resto igual a zero, então cont passa para 2, em seguida, 4/3 não terá resto igual a zero, em seguida, 4/4 terá resto igual a zero, logo cont passa para três. Logo, cont não é igual a 2, deste modo, não é um primo.


## Questão 04
Considere o código a seguir onde temos uma estrutura de repetição for. int x=4, y = 8, r=0;

 

  for(int i=0; i<x;i++)

   r=r+y;

  System.out.println(r);

Considerando as informações apresentadas neste código-fonte, avalie as afirmações a seguir:

I. O código apresentará um erro na linha 3, pois a condição de parada deve conter um número após o sinal de menor.

II. O resultado deste código será a multiplicação do valor da variável x pelo valor da variável y, totalizando 32.

III. O valor da variável y será somado com o valor da variável r, deste modo, será apresentado o valor 8 na linha 5.

IV. O resultado deste código será uma exponenciação se mudarmos o valor de r para 1 e substituirmos a soma por multiplicação.

Estão corretas apenas as afirmativas:

### Resposta:
- a) II e IV, apenas

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra A, pois a afirmativa I está incorreta, afinal, a condição de parada é i<x, onde x é a variável declarada previamente. A afirmativa II é verdadeira, note que a soma será repetida em um número determinado de vezes, ou seja, x vezes. A afirmativa III está incorreta, pois a soma da variável y com a variável r acontece em função de x, logo, o resultado não será 8, mas sim, 32. A afirmativa IV está correta, pois realizando estas alterações, vamos multiplicar a variável y por r em um número x de vezes.
