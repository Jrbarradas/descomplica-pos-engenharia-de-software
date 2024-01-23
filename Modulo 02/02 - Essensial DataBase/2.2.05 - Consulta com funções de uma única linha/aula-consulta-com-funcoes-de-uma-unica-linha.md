# Consultas com funções de uma única linha

# Exercícios


## Questão 01
Você criou um relatório para apresentar os preços dos produtos de seu estoque. Qual comando você usa para apresentar os preços no formato “$0.25”?

![Fonte: autoral, 2023.](https://paperx-dex-assets.s3.sa-east-1.amazonaws.com/images/1683584199737-9WRSbFL0AA.png)

Fonte: autoral, 2023.

### Resposta:
- e) ​ SELECT TO_CHAR(price, ‘$999990.99’)

  ​                   FROM inventory;

> SOLUÇÃO DO PROFESSOR ✨
>
> É necessário converter o número para um caracter, por isso, usa-se a função to_char e o campo price tem 8 dígitos.


## Questão 02
Analise este comando:

SELECT *
FROM product
WHERE LOWER(description) = ‘CABLE’;

Que resultado este comando apresentará?

### Resposta:
- a) Irá executar, mas não recuperar dados

> SOLUÇÃO DO PROFESSOR ✨
>
> Não irá recuperar dados pois está comparando uma string em letra minúscula com uma string em letra maiúscula.


## Questão 03
Você tenta consultar o banco de dados com o seguinte comando

**SELECT 100/NVL(quantity, 0)**

**FROM inventory;**

Por que este comando causa um erro quando o valor de QUANTITY é nulo?

### Resposta:
- a) A expressão tenta dividir por zero

> SOLUÇÃO DO PROFESSOR ✨
>
> A função NVL converte o nulo para o valor 0. Portanto, o comando tenta fazer uma divisão por zero.


## Questão 04
Você consulta o banco de dados com o seguinte comando:

**SELECT CONCAT(UPPER(SUBSTR(location, 1, 3)), dept_number) “Department Location”**

**FROM department;**

Que função é avaliada por último?

### Resposta:
- b) CONCAT

> SOLUÇÃO DO PROFESSOR ✨
>
> Quando existe um aninhamento de funções a função mais externa é a última a ser executada.

