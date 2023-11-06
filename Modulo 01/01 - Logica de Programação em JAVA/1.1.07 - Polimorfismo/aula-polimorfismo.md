# Polimorfismo

# Exercícios


## Questão 01
A palavra polimorfismo significa muitas formas. Vem da palavra grega poli (significa muitos) e morphos (significa forma). Por exemplo, em química, o carbono exibe polimorfismo porque pode ser encontrado em mais de uma forma: grafite e diamante. Mas, cada uma das fórmulas tem suas próprias propriedades distintas.
A partir desta definição de polimorfismo, qual alternativa apresenta três maneiras de sobrecarga de métodos?

### Resposta:
- b) número de parâmetros, tipos de dados dos parâmetros, ordem dos tipos de dados de parâmetros

> SOLUÇÃO DO PROFESSOR ✨
>
> A sobrecarga visa criar variações de um método, logo, o nome é igual, o que modifica são os parâmetros, tanto em número, tipo quanto em ordem.


## Questão 02
Digamos que temos uma classe Animal que tem um método chamado som(). Como esta é uma classe genérica, não podemos dar uma implementação como: miar, latir, rosnar, entre outros sons de diferentes animais. Supondo que existem duas classes, uma chamada cachorro e outra chamada gato que herdam da classe animal, cada uma possui em seu escopo respectivamente as mensagens System.out.println(“latindo…”); e System.out.println(“miando…”);. Considerando que o nome do método som() não foi modificado, mas somente seu conteúdo, temos um exemplo de (marque a alternativa correta)

### Resposta:
- b) polimorfismo, mais especificamente sobrescrita pois temos os métodos com a mesma assinatura

> SOLUÇÃO DO PROFESSOR ✨
>
> O polimorfismo é um dos recursos de Programação Orientada a Objetos que nos permite realizar uma única ação de diferentes maneiras. Neste caso, o método continua com o mesmo nome e estrutura de parâmetros (mesma assinatura) e estamos apenas modificando o comportamento dele, ou seja, seu escopo. Logo, trata-se de sobrescrita


## Questão 03
A herança em java envolve um relacionamento entre as classes pai e filha. Sempre que ambas as classes contiverem métodos com o mesmo nome e parâmetros, é certo que um dos métodos substituirá o outro método durante a execução. O método que será executado depende do objeto.
Considere esta hierarquia onde uma classe filha herda os métodos e atributos de uma classe pai. Tanto a classe pai quanto a classe filha tem um método chamado calcular(). Qual alternativa melhor descreve a execução deste programa?

### Resposta:
- c) se o objeto da classe filho chamar o método calcular(), o método da classe filho substituirá o método da classe pai

> SOLUÇÃO DO PROFESSOR ✨
>
> Por substituição (overriding), o método da classe filha será executado, substituindo o método da classe pai


## Questão 04
Polimorfismo é uma palavra que significa várias formas. Considere, por exemplo, uma classe chamada Pessoa. Nesta classe, dentre os diversos métodos, temos um chamado correr, o qual recebe dois parâmetros do tipo inteiro; temos também um método chamado aferirVelocidade, o qual possuí apenas 1 atributo do tipo inteiro. A classe chamada Corredor é um tipo de Pessoa e possuí o método correr com dois parâmetros do tipo inteiro e dois parâmetros do tipo double; o método aferirVelocidade da classe Corredor possui apenas 1 atributo do tipo inteiro. Sobre estes métodos, é correto dizer: (marque a alternativa correta)

### Resposta:
- a) Existe sobrecarga no método correr, pois a assinatura é diferente

> SOLUÇÃO DO PROFESSOR ✨
>
> A assinatura do método sobrecarregado deve ser diferente, observe que os parâmetros do método correr são diferentes. Por outro lado, na sobrescrita a assinatura do método deve ser a mesma

