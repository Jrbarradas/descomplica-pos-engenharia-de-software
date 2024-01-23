# Linguagem SQL - Comandos DML e DQL

# Exercícios


## Questão 01
Estabeleça a relação entre os elementos das duas colunas da tabela abaixo.

![img](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1683584845231-PJA8jSYjYN.png)

Marque a opção que representa a relação correta:

### Resposta:
- e) 1-c, 2-a, 3-b, 4-d

> SOLUÇÃO DO PROFESSOR ✨
>
> 1. SELECT – Seleciona as colunas do resultado ©
> 2. FROM – Define a tabela a ser consultada (a)
> 3. WHERE – Contém as condições de seleção de linhas (b)
> 4. DISTINCT – Inclui no resultado apenas linhas distintas (d)


## Questão 02
Após ser feita a seguinte consulta ao banco de dados:

SELECT price

FROM INVENTORY

WHERE price BETWEEN 1 AND 50

And price BETWEEN 25 AND 75);

 

Qual valor está SELECT poderia recuperar?

### Resposta:
- a) 30

> SOLUÇÃO DO PROFESSOR ✨
>
> O valor do campo price deve se encaixar nas duas condições estipuladas, ou seja, deve estar entre 1 até 50 E entre 25 até 75, das alternativas o único valor que adequa as condições estabelecidas é o 30.


## Questão 03
Para que tarefa você usa a cláusula WHERE numa SELECT?

### Resposta:
- b) Para comparar os valores armazenados numa coluna com um determinado valor

> SOLUÇÃO DO PROFESSOR ✨
>
> A cláusula where é usada para comparar os valores armazenados numa coluna com um determinado valor.


## Questão 04
Analise o comando abaixo:

Update dept
Set dname=’COMERCIAL’;

Quantas linhas da tabela dept serão afetadas por esse comando?

### Resposta:
- a) Todas

> SOLUÇÃO DO PROFESSOR ✨
>
> Quando o comando update não possui a restrição da cláusula where, todas as linhas da tabela são afetadas pela alteração.

