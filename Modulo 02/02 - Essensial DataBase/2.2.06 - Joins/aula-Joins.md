# Joins

# Exercícios


## Questão 01
Analise a consulta SQL abaixo:

SELECT      e.name, e.employee_id, e.department_id, d.location

FROM       employee e join department d

ON          employee.department_id = department.department_id

ORDER BY   e.name;

Esta consulta falhará quando executada. Que mudança corrigirá o problema?

### Resposta:
- c) Use apelido de tabelas ao invés de nomes de tabelas na cláusula ON

> SOLUÇÃO DO PROFESSOR ✨
>
> Se os apelidos de tabelas foram definidos, é necessário usar esses apelidos em todas as outras cláusulas.


## Questão 02
Analise a consulta abaixo:

SELECT          i.id_number, m.manufacturer_id

FROM            inventory I join inventory m

ON             i.manufacturer_id = m.region_id_number;

Qual é o tipo de junção feito acima?

### Resposta:
- d) autojunção

> SOLUÇÃO DO PROFESSOR ✨
>
> A união da tabela com ela mesma é a definição de uma autojunção.


## Questão 03
Analise a consulta abaixo:

SELECT e.ename, d.dname

FROM scott.emp e JOIN scott.dept d

ON (e.deptno = d.deptno;

Qual é o tipo de junção feito acima?

### Resposta:
- a) junção idêntica

> SOLUÇÃO DO PROFESSOR ✨
>
> A junção idêntica é caracterizada pela presença do sinal de = na condição da junção.


## Questão 04
Para se realizar uma junção envolvendo cinco tabelas, quantas condições de junção devem ser estipuladas?

### Resposta:
- b) 4

> SOLUÇÃO DO PROFESSOR ✨
>
> Se n representa o número de tabelas, n-1 deve ser o número de condições de junção.

