# Módulo 2 - Avaliação Estudo de Caso

Nome completo: Paulo Sérgio de Macedo Barradas Júnior
Curso: Pós-Graduação em Engenharia de Software
Área: Tecnologia Nº do estudo de caso: 91
Lembretes importantes:
• Leia o manual para elaboração de estudo de caso;
• Não é necessário reproduzir o enunciado do estudo de caso;
• Não se preocupe com a ABNT! Seu trabalho pode seguir este template (fonte Arial, tamanho 12 com espaçamento simples);
• O estudo de caso deve ter no mínimo 400 e máximo de 800 palavras contando a partir do título.
Análise Avançada com SQL na Cult Livros



1. Preço Máximo de um livro na Cult Livros:

  ​	Com base nas tabelas propostas, o preço máximo de um livro na Cult Livros é indeterminado e altamente variável. A coluna preco na tabela Livros é do tipo decimal (5,2), o que significa que pode armazenar valores decimais com até 5 dígitos inteiros e 2 casas decimais. No entanto, não há restrição de valor máximo, permitindo que a Culti Livros defina livremente os preços, resultando em preços possivelmente muito altos. Não há restrição na definição da coluna que limite o valor máximo que pode ser armazenado.
  ​	Isso significa que a Cult Livros pode ter livros com preços muito altos, dependendo da estratégia de precificação da empresa. É importante ressaltar que, do ponto de vista técnico, a coluna preco suporta valores até 99.999,99.

2. Livros em baixa no estoque, com menos de 10 livros:

  ​	A seguinte consulta SQL identifica quais livros na Cult Livros estão em baixa no estoque, com menos de 10 unidades e utilizando o CASE WHEN gera uma classificação de status para facilitar a análise e utilização do ORDER BY para ordenação dos resultados por quantidade em estoque crescente para priorizar os livros com menor quantidade.

  ​										Consulta SQL

  SELECT titulo, autor, categoria, quantidade_em_estoque,
  CASE
  WHEN quantidade_em_estoque < = 5 THEN ‘Estoque Crítico!’
  WHEN quantidade_em_estoque < = 10 THEN ‘Estoque Baixo’
  ELSE ‘Estoque Suficiente’
  END AS status_estoque
  FROM Livros
  WHERE quantidade_em_estoque < 10
  ORDER BY quantidade_em_estoque ASC;

3. Quantidade em estoque do livro com id = 99 após a venda de uma unidade:

  ​	Para atualizar a quantidade em estoque do livro com ID 99 após a venda de uma unidade, utilizaremos a seguinte consulta SQL:

  ​										Consulta SQL

  UPDATE Livros
  SET quantidade_em_estoque = quantidade_em_estoque -1
  WHERE id = 99;

  ​										Conclusão

  ​	O SQL é uma ferramenta poderosa para gerenciar e analisar dados de forma eficiente a Cult Livros.
  ​	É fundamental garantir a segurança do banco de dados da Cult Livros, implementando medidas como autenticação, criptografia e controle de acesso. Implementar um plano de backup regular para garantir a recuperação de dados em caso de falhas ou eventos inesperados.
  ​	O sistema de banco de dados deve ser capaz de lidar com o crescimento do volume de dados da Cult Livros.
  ​	O sistema de gerenciamento de estoque precisa se integrar com outros sistemas da livraria, como o sistema de vendas e o sistema financeiro.
  ​	É necessário garantir a manutenção e atualização regular do sistema de banco de dados para garantir sua segurança e desempenho.
  ​	A equipe Cult Livros precisa ser treinada para utilizar o sistema de forma eficiente.

<hr>
SOLUÇÃO DO PROFESSOR ✨

Sua nota: **10.0****/10**

Detalhes: **Forma e apresentação**

Apresentação Valendo até 2.0

Nota: 2.0

Aderência Valendo até 2.0

Nota: 2.0

Contextualização Valendo até 2.0

Nota: 2.0

Problematização Valendo até 2.0

Nota: 2.0

Solução Valendo até 2.0

Nota: 2.0

**Comentário do tutor**

O aluno apresentou um texto estruturado, dividido em introdução, desenvolvimento e conclusão. Além disso, utilizou uma linguagem clara e adequada. O aluno alinhou o tema do estudo de caso com sua área de atuação, que é a Tecnologia. O aluno contextualizou o problema apresentado no estudo de caso, explicando a situação atual da Cult Livros e as dificuldades que enfrentam em gerenciar seu estoque de forma eficiente. O aluno definiu a pergunta da pesquisa de forma específica, abordando o problema da Cult Livros em gerenciar seu estoque de forma eficiente. Além disso, condensou as ideias sobre a problematização, apresentando pontos-chave e teorizando sobre a aplicação na realidade. O aluno apresentou opiniões com argumentos concretos, construindo a ideia em um texto dissertativo. Além disso, utilizou exemplos para justificar sua base de solução e apresentou o desenvolvimento da ideia até uma solução final.

## 