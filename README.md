# Orientacao-a-objetos
Um breve resumo a respeito dos 4 pilares da Programação Orientada a Objetos.

## Introdução
  Bem-vindo ao meu artigo sobre os 4 pilares da orientação a objetos! Nele, discutiremos os conceitos principais que compõem a base da programação orientada a objetos (POO). Os 4 pilares são princípios-chave que norteiam o design e a implementação de sistemas baseados em objetos, permitindo a flexibilidade, reutilização e a manutenibilidade de código.

## Pilares da POO

### Encapsulamento

 Na Programação Orientada a Objetos (POO), a prática comum é encapsular dados e métodos dentro de classes. Mas o que exatamente significa encapsular métodos e dados? Os atributos e métodos de uma classe estão estreitamente interligados. Embora os objetos possam se comunicar entre si, geralmente não têm conhecimento sobre a implementação interna de outros objetos, pois esses detalhes permanecem ocultos dentro do próprio objeto. Abaixo, veremos um modelo de encapsulamento:
 ![Encapsulamento](https://github.com/VictorOliveira28/Orientacao-a-objetos/raw/main/imagens/Encapsulamento.png)

 ### Herança
  Na Programação Orientada a Objetos (POO), a herança é um mecanismo que permite que uma classe herde as características (atributos e métodos) de uma outra classe. Essa abordagem possibilita a reutilização de código e estabelece uma relação "é-um" entre as classes. A classe derivada (classe filha) herda as propriedades da classe base (classe pai). Veremos a seguir um exemplo de Herança:

  Neste contexto, desenvolvemos a classe pai, responsável por fornecer os atributos e métodos fundamentais à classe filha.
  ![Herança](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a1.png)

  Posteriormente, implementamos a classe filha, que herda integralmente os métodos e atributos da classe pai.
  ![Herança](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a2.png)
  É importante notar que a classe SavingsAccount herda os seguintes atributos da classe pai:

accountNumber: Identificador exclusivo da conta.

accountHolder: Nome do titular da conta.

balance: Saldo atual da conta.

Além disso, a classe SavingsAccount herda os seguintes métodos:

deposit(double amount): Adiciona um valor ao saldo da conta.

withdraw(double amount): Retira um valor do saldo da conta, garantindo que haja fundos suficientes.

displayBalance(): Apresenta o saldo atual da conta.

A classe SavingsAccount também incorpora atributos e métodos próprios:

interestRate: Taxa de juros associada à conta de poupança.

addInterest(): Calcula e adiciona juros à conta com base na taxa de juros configurada.

### Polimorfismo

Polimorfismo permite que objetos de diferentes classes sejam tratados de maneira uniforme. Existem dois tipos de polimorfismo: estático (sobrecarga de método) e dinâmico (sobreposição de método). O polimorfismo aumenta a flexibilidade e facilita a manutenção do código. Observe o código a seguir:

![Polimorfismo](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/Captura%20de%20tela%202024-01-16%20145157.png)

Neste exemplo em Java, a função performTransaction é capaz de processar qualquer objeto que seja do tipo Account, o que inclui objetos da classe derivada SavingsAccount. Esse cenário ilustra o conceito de polimorfismo, possibilitando a execução de operações comuns em distintos tipos de contas.

### Abstração

A abstração compreende a simplificação de complexidades desnecessárias, concentrando-se nos aspectos essenciais do objeto. Classes e interfaces são empregadas para representar entidades abstratas do mundo real. Esse conceito permite aos desenvolvedores ignorar detalhes irrelevantes e direcionar sua atenção para o que é crucial na aplicação.
Irei utilizar novamente o exemplo da Account e SavingsAccount para exemplificar a abstração.

A classe Account oferece uma abstração para uma conta bancária genérica, apresentando métodos como withdraw e displayBalance, que representam ações comuns em contas. Já a classe SavingsAccount estende a Account e acrescenta um comportamento específico para contas de poupança, introduzindo o método addInterest para calcular e adicionar juros à conta.
![Abstração](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a1.png)
 

 Ao chamar a função performTransaction, você está utilizando a abstração proporcionada pela classe Account para efetuar transações, sem considerar se é uma conta comum ou uma conta poupança. Isso exemplifica o conceito de abstração, no qual objetos de classes distintas são tratados de maneira uniforme, utilizando apenas a interface comum fornecida pela classe base (Account). 
 ![Abstração](https://github.com/VictorOliveira28/Orientacao-a-objetos/blob/main/imagens/heran%C3%A7a2.png)

 ## Conclusão

Em conclusão, ao compreender e aplicar os pilares da POO, os desenvolvedores podem criar sistemas mais eficientes, flexíveis e fáceis de manter. A combinação de encapsulamento, herança, polimorfismo e abstração constitui uma base sólida para o desenvolvimento de software orientado a objetos, impulsionando a inovação e a eficácia no mundo da programação.



 
