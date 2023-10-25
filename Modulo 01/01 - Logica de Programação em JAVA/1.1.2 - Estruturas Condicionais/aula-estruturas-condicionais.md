# Estruturas Condicionais

# Exercícios


## Questão 01
Analise com atenção o código a seguir:

Int a = 41;

Int b = 9;

Int aux;

If(a>b){

aux = a;

a = b;

b = aux;

}

System.out.println(“O valor da variável a é:” + a);

System.out.println(“O valor da variável b é:” + b);

Considerando as informações apresentadas neste código, assinale a opção correta.

### Resposta:
- e) O objetivo deste código é apresentar uma sequência ordenada nas linhas 9 e 10, e a linha 5 é essencial neste processo

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra E, pois este algoritmo é responsável por realizar a troca dos valores contidos nas variáveis a e b sempre que encontrar um valor de a que seja maior que o valor de b. Este é o princípio de um algoritmo de ordenação. Observe que, se for realizada uma troca direta, ou seja, se a receber o valor de b, o valor de a será perdido. Logo, é necessário salvar em aux (uma variável temporária) o valor da variável a, e em seguida realizar as trocas. No fim, a variável b recebe aux, ou seja, recebe o valor antigo de a.


## Questão 02
O código a seguir realiza a validação se um ano é bissexto ou não. Para este cálculo alguns critérios devem ser respeitados: 1) o ano deve ser divisível por quatro, 2) o resto da divisão do ano por 100 tem que ser maior que zero, 3) ou a divisão do ano por 400 precisa ser igual a zero. Análise o código com atenção.     

int ano = 2000;

if(((ano % 4) == 0 || (ano%100)>0) || ((ano%400) == 0)){

System.out.println(“Ano bissexto”);

} else {

System.out.println(“Ano não é bissexto”);

}

Considerando esse código, avalie as alternativas a seguir e marque a correta.


### Resposta:
- c) Na linha 3, o valor da expressão será true para qualquer ano maior que 1500, uma vez que temos um operador ou (II), tornando a linha 6 inalcançável.

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra C, pois como temos operador ou (II), o resultado será verdadeiro para qualquer valor de entrada da linha 3, logo, a linha 6 não será executada.


## Questão 03
Observe com atenção o código a seguir, o qual se assemelha a um controle de acesso de um usuário em um sistema qualquer, solicitando um nome de usuário que será armazenado na variável txt.

String txt;

if(txt !=”Maria”){

 System.out.println(txt + “seu acesso não está autorizado”);

} else {

  System.out.println(txt + “seu acesso foi autorizado”);

 System.out.println(“...”);

}

Marque a alternativa que corretamente explica sobre a execução deste código. 

### Resposta:
- c) se o usuário digitar um valor na linha 1 deste código e este valor for armazenado variável txt, ele será apresentado na linha 4 ou na linha 6

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra C, pois na linha 1 0 usuário entrará com um valor que, conforme solicitado, deve ser um nome para a variável txt. Se o nome for diferente de Maria, então será apresentado o valor da linha 4, caso contrário, será apresentado o valor da linha 6.


## Questão 04
Considere o trecho de código a seguir onde temos 3 variáveis declaradas previamente.


 String valorA = “true”;

boolean valorB = true;
 boolean valorC = true;

if(valorA == "true"){

System.out.println(“Valor da variável valorA é true”);
 }
 if(valorB == true){

System.out.println(“Valor da variável valorB é true”);

}
 if(valorC){

System.out.println(“Valor da variável C é false”);

}

Considerando as informações apresentadas neste código-fonte, avalie as afirmações a seguir:

 I. Como o valor da variável valorA é True, então a comparação na linha 5 será verdadeira e será apresentado o conteúdo da linha 6 na tela.

II. Haverá um erro no código na linha 11 pois não há uma comparação da variável valorC com um outro valor ou variável.

III. Na tela serão apresentados os conteúdos das linhas 9 e 12, pois valorC e valorB são iguais a True.

IV. Existem dois tipos diferentes de variáveis neste código, sendo um tipo string e um tipo inteiro.

 Estão corretas apenas as afirmativas:

### Resposta:
- e) I e III, apenas

> SOLUÇÃO DO PROFESSOR ✨
>
> Letra E, pois a afirmativa III é verdadeira, afinal as variáveis valorB e valorC recebem um dado do tipo booleano, logo, são valores lógicos que podem ser comparados com valores do mesmo tipo no código. No caso da linha 11, quando não há um sinal de comparação, entende-se que, e aquela variável ou expressão tiver um conteúdo True, então executa o escopo do if. A afirmativa IV é verdadeira, pois a variável valorA é do tipo string e as variáveis valorB e valorC são do tipo booleano, logo, temos dois tipos de variáveis.

