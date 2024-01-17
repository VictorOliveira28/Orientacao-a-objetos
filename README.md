# Orientacao-a-objetos
Um breve resumo a respeito dos 4 pilares da Programação Orientada a Objetos.

## Introdução
  Neste resumo, discutiremos os conceitos principais que compõem a base da programação orientada a objetos (POO), Encapsulamento, Herança, Polimorfismo e Abstração. Os 4 pilares são princípios-chave que norteiam o design e a implementação de sistemas baseados em objetos, permitindo a flexibilidade, reutilização e a manutenibilidade de código.

## Pilares da POO

### Encapsulamento

 Na Programação Orientada a Objetos (POO), a prática comum é encapsular atributos e métodos dentro de classes. Mas o que exatamente significa encapsular métodos e atributos? Encapsular é restringir o acesso a uma informação, conforme a necessidade do projeto, mas lembre-se, encapsular não significa tornar a informação inacessível, mas controlar como essa informação é acessada. A ideia é que objetos externos não precisam conhecer os detalhes internos de outro objeto, isso quer dizer que a implementação interna de um objeto é oculta para outros. Esse encapsulamento ocorre na estrutura interna do objeto, incluindo seus métodos e atributos privados, mantendo dentro do escopo do próprio objeto. A utilização dos modificadores de acesso é essencial para implementar o encapsulamento, eles definem as regras de visibilidade dos membros de uma classe, determinando quem pode acessar e/ou modificar determinadas partes do código.
 
 Abaixo, veremos um modelo de encapsulamento:
 ![Encapsulamento](https://github.com/VictorOliveira28/Orientacao-a-objetos/raw/main/imagens/Encapsulamento.png)

 ### Herança
 
  Na Programação Orientada a Objetos (POO), a herança é um mecanismo que permite que uma classe herde as características (atributos e métodos) de uma outra classe. Essa abordagem possibilita a reutilização de código e estabelece uma relação "é-um" entre as classes. A classe derivada (classe filha) herda as propriedades da classe base (classe pai).
  Veremos a seguir um exemplo de Herança:

  Neste contexto, desenvolvemos a classe pai, responsável por fornecer os atributos e métodos fundamentais à classe filha.
  ![Herança](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a1.png)
  ![Herança](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/Captura%20de%20tela%202024-01-17%20114720.png)

  Posteriormente, implementamos a classe filha, que herda integralmente os métodos e atributos da classe pai.
  ![Herança](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a2.png)
  É importante notar que a classe SavingsAccount herda (esse recurso se da pela palavra reservada extends, que informa ao compilador sobre a operação de herança) os seguintes atributos da classe pai:

number: Identificador exclusivo da conta.

holder: Nome do titular da conta.

balance: Saldo atual da conta.

Além disso, a classe SavingsAccount herda os seguintes métodos:

deposit(double amount): Adiciona um valor ao saldo da conta.

withdraw(double amount): Retira um valor do saldo da conta, garantindo que haja fundos suficientes.

displayBalance(): Apresenta o saldo atual da conta.

A classe SavingsAccount também incorpora atributos e métodos próprios:

interestRate: Taxa de juros associada à conta de poupança.

addInterest(): Calcula e adiciona juros à conta com base na taxa de juros configurada.

A decisão de usar herança deve ser baseada nas necessidades específicas do seu projeto e na estrutura mais eficiente e fácil de se manter. No entanto, é importante ter cuidado ao utilizar Herança, considerando os desafios e problemas associados a ela, como rigidez na estrutura, forte acoplamento e poluição de interfaces. Alguns programadores preferem utilizar Composições e Interfaces, pois elas aumentam a flexibilidade e manutenabilidade do código.

### Polimorfismo

Polimorfismo permite que objetos assumam diferentes formas, uma mesma operação pode ser realizada por diferentes objetos de classes diferentes. Podemos implementar o polimorfismo através do uso de herança e interfaces. Com isso, podemos criar códigos mais genéricos e flexíveis, tornando o processo de desenvolvimento mais eficiente. Compreender oque é o polimorfismo é essencial para quem quer desenvolver aplicações de qualidade e com alta performance.
Abaixo veremos um exemplo de polimorfismo:

![Polimorfismo](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/Captura%20de%20tela%202024-01-16%20145157.png)

Neste exemplo em Java, a função performTransaction é capaz de processar qualquer objeto que seja do tipo Account, o que inclui objetos da classe derivada SavingsAccount. Esse cenário ilustra o conceito de polimorfismo, possibilitando a execução de operações comuns em distintos tipos de contas.

### Abstração

A abstração compreende a simplificação de complexidades desnecessárias, concentrando-se nos aspectos essenciais do objeto. Classes e interfaces são empregadas para representar entidades abstratas do mundo real. Esse conceito permite aos desenvolvedores ignorar detalhes irrelevantes e direcionar sua atenção para o que é crucial na aplicação.
Irei utilizar novamente o exemplo da Account e SavingsAccount para exemplificar a abstração.

A classe Account oferece uma abstração para uma conta bancária genérica, apresentando métodos como withdraw e displayBalance, que representam ações comuns em contas. Já a classe SavingsAccount estende a Account e acrescenta um comportamento específico para contas de poupança, introduzindo o método addInterest para calcular e adicionar juros à conta.

![Abstração](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a1.png)
 

 Ao chamar a função performTransaction, você está utilizando a abstração proporcionada pela classe Account para efetuar transações, sem considerar se é uma conta comum ou uma conta poupança. Isso exemplifica o conceito de abstração, no qual objetos de classes distintas são tratados de maneira uniforme, utilizando apenas uma operação comum fornecida pela classe base (Account).
 
 ![Abstração](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a2.png)

 ## Conclusão

Ao compreender e aplicar os pilares da POO, os desenvolvedores podem criar sistemas mais eficientes, flexíveis e fáceis de manter. A combinação de encapsulamento, herança, polimorfismo e abstração constrói uma base sólida para o desenvolvimento de software orientado a objetos, impulsionando a inovação e a eficácia no mundo da programação.



Livro:
Deitel, P., & Deitel, H. (2014). Java 8: Como Programar. 

Artigo Online:
DevMedia. (2018). Uso de polimorfismo em Java. Disponível em: https://www.devmedia.com.br/uso-de-polimorfismo-em-java/26140.

AWARI. (2024). Polimorfismo em Java. Disponível em: https://awari.com.br/polimorfismo-em-java/.
