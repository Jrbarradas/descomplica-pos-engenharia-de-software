# Funções de grupo e subconsultas

# Exercícios


## Questão 01
Que cláusula é usada para restringir valores retornados por uma função de grupo?

### Resposta:
- b) HAVING

> SOLUÇÃO DO PROFESSOR ✨
>
> A cláusula having é usada para restringir valores retornados por uma função de grupo.


## Questão 02
Para que resultado você utilizaria uma função de grupo?

### Resposta:
- c) Para produzir o total de todos os valores da coluna CUSTO da tabela PRODUTO

> SOLUÇÃO DO PROFESSOR ✨
>
> A função de grupo SUM, faz o somatório de um campo.


## Questão 03
Qual declaração SELECT apresentará o número de itens que tenham o valor de PRICE maior que 5.00?

![img](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1683582004870-KPMDYEPYHn.png)

### Resposta:
- c)  SELECT               COUNT(*)

  ​                  FROM inventory

  ​                      WHERE                 price > 5.00

> SOLUÇÃO DO PROFESSOR ✨
>
> Para contar a quantidade, deve-se usar a função de grupo COUNT.


## Questão 04
Analise o comando abaixo:

SELECT        manufacturer_id, AVG(price)

FROM                 inventory

WHERE            AVG(price) > 6.00

GROUP BY          manufacturer_id

ORDER BY            AVG(price);

Qual linha causará um erro?

### Resposta:
- b) WHERE AVG(price) > 6.00

> SOLUÇÃO DO PROFESSOR ✨
>
> Para restringir a função de grupo devemos utilizar a cláusula Having.

