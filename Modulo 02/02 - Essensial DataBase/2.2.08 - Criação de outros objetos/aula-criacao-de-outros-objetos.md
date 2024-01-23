# Criação de outros objetos

# Exercícios


## Questão 01
Analise o seguinte comando:

CREATE VISÃO (VIEW) parts_vu(company,contact)
AS SELECT manufacturer_name, contact_name
FROM inventory
WITH READ ONLY;

Qual comando pode ser utilizado na visão (view) PARTS_VU:

### Resposta:
- c) SELECT

> SOLUÇÃO DO PROFESSOR ✨
>
> Em uma visão (view) criada com a opção de with read only, só são permitidas operações de leitura.


## Questão 02
Examine o visão (view) EMP_HIST_V:

 

EMP_HIST_V

 

Name           Type

--------------------    -----------------------------------

EMPLOYEE_ID        NUMBER(6)

NAME          VARCHAR2(15)

JOB            VARCHAR2(9)

MANAGER       NUMBER(4)

DATE_HIRED          DATE

SALARY         NUMBER(7,2)

BONUS         NUMBER(7,2)

DEPARTMENT_ID NUMBER(2)

 

Você precisa consultar a visão (view) acima para determinar o salário médio de todos empregados que atuam no setor 10 que foram contratados antes de 01 de janeiro de 1995. Qual consulta você usaria?

### Resposta:
- d) SELECT         department_id, AVG(salary)

  FROM           emp_hist_v

  WHERE    date_hired < ’01-JAN-1995’

  AND       department_id = 10

  GROUP BY department_id;

-  

> SOLUÇÃO DO PROFESSOR ✨
>
> Uma visão (view) complexa suporta a utilização de função de grupo.


## Questão 03
Qual a consulta que não terá sucesso na consulta da visão (view) EMP_HIST_V?

 

Name           Type

--------------------    -----------------------------------

EMPLOYEE_ID        NUMBER(6)

NAME          VARCHAR2(15)

JOB            VARCHAR2(9)

MANAGER       NUMBER(4)

DATE_HIRED          DATE

SALARY         NUMBER(7,2)

BONUS         NUMBER(7,2)

DEPARTMENT_ID NUMBER(2)

### Resposta:
- a) SELECT *

  ​     FROM VISÃO (VIEW) emp_hist_v;

> SOLUÇÃO DO PROFESSOR ✨
>
> Não é necessário colocar na cláusula from a palavra visão (view), para se fazer uma consulta em uma visão.


## Questão 04
 Avalie o seguinte comando:

 

CREATE SEQUENCE line_item_id

​     START WITH 10001

​     MAXVALUE 999999999

​     NOCYCLE;

 

Qual afirmativa sobre o comando CREATE SEQUENCE acima é verdadeira?

### Resposta:
- b) A sequência nunca reutilizará qualquer código e será incrementada de 1 a cada chamada

> SOLUÇÃO DO PROFESSOR ✨
>
> Por conta da cláusula NOCYCLE, ou seja, não cíclica, a sequência nunca reutilizará qualquer código.

