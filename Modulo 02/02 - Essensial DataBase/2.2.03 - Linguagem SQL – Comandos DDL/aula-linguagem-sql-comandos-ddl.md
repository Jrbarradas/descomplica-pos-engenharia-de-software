# Linguagem SQL - Comandos DDL

# Exercícios


## Questão 01
Para criarmos uma tabela, utilizamos o comando CREATE TABLE, já para alterarmos a estrutura de uma tabela utilizamos o comando ALTER TABLE e para excluirmos uma tabela usamos o comando DROP TABLE. Pensando nesse conceito, analise as afirmativas abaixo.

I.ALTER TABLE
II.ADD COLUMN
III.CREATE COLUMN
IV.MODIFY COLUMN
V. ALTER COLUMN
Baseando-se em sua análise, informe qual comando permite adicionar um campo a tabela?

### Resposta:
- a) ​I

> SOLUÇÃO DO PROFESSOR ✨
>
> O Comando que permite adicionar uma coluna a uma tabela existente é o comando Alter Table, add column não existe.


## Questão 02
Você precisa eliminar de forma definitiva o conteúdo e a estrutura da tabela EMP do banco de dados. Para realizar tal tarefa, qual comando você deve realizar?

### Resposta:
- a) DROP TABLE EMP;

> SOLUÇÃO DO PROFESSOR ✨
>
> O Comando que permite a exclusão de conteúdo e estrutura da tabela é o comando DROP TABLE.


## Questão 03
Os atributos do tipo chave primária possuem uma importância única e representam dados que:

### Resposta:
- d) Não podem ser nulos nem mesmo se repetir

> SOLUÇÃO DO PROFESSOR ✨
>
> A chave primária em um banco de dados é um atributo ou um conjunto de atributos que identifica de forma única cada registro em uma tabela. Por esse motivo, ela possui duas características principais:
> • Unicidade: A chave primária não pode ter valores repetidos. Isso garante que cada registro na tabela possa ser identificado de forma exclusiva. Se a chave primária fosse repetida, não haveria como distinguir registros diferentes.
> • Não nulidade: A chave primária não pode ser nula. Uma vez que a função da chave primária é identificar cada registro, um valor nulo invalidaria essa função, pois não seria possível identificar um registro sem uma chave primária válida.
> As demais opções falham em cumprir um ou ambos desses critérios:
> • a: Se uma chave primária pudesse se repetir, não seria possível garantir a identificação única de cada registro.
> • b: Chaves primárias não podem ser nulas.
> • c: Novamente, a repetição de valores na chave primária impede a identificação única.
> • e: Ainda que as chaves primárias sejam identificadores, sua característica não é ser comum, mas ser única para cada registro.
> Portanto, a opção que descreve corretamente as propriedades de uma chave primária em um banco de dados é a que diz: Não podem ser nulos nem mesmo se repetir.


## Questão 04
Qual comando deve ser usado para inserir uma constraint de chave estrangeira (foreign key – FK), na tabela
I.ALTER TABLE
II.ADD CONSTRAINT
III.INSERT CONSTRAINT
IV.MODIFY CONSTRAINT
V. ALTER COLUMN CONSTRAINT

### Resposta:
- a) I

> SOLUÇÃO DO PROFESSOR ✨
>
> O Comando que permite adicionar uma constraint a uma tabela existente é o comando Alter Table, add constraint é uma cláusula do comando ALTER TABLE.

