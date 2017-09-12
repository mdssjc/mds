# GoF

O acrônimo GoF - _Gang of Four_ apresentado no livro _Design Patterns_ dos autores _Erich Gamma_,
 _John Vlissides_, _Ralph Jonhson_ e _Richard Helm_ explana um catálogo de 23 genéricas soluções para o desenvolvimento de _software_ no paradigma orientado a objetos.

Os _Design Patterns_ do livro são: "_descrições de objetos e classes comunicantes que precisam ser personalizadas para resolver um problema geral de projeto num contexto particular_".

Os princípios por trás dos padrões estão:

* **Programe para uma interface, não para uma implementação** - _Program to an interface, not to an implementation_: introduzido no livro do GoF, recomenda o uso de abstrações como ponto de acesso entre elementos de programação.
* **Prefira a composição de objeto à herança de classe** - _Favor object composition over class inheritance_: introduzido no livro do GoF, recomenda o uso de composição à herança na construção elementos de programação.

Classificação segundo GoF:

 |            |            |                  | **Propósito**    |                         |
 |------------|------------|------------------|------------------|-------------------------|
 |            |            | **Criação**      | **Estrutura**    | **Comportamento**       |
 |            |            | _Creational_     | _Structural_     | _Behavioral_            |
 |------------|------------|------------------|------------------|-------------------------|
 | **Escopo** | **Classe** | Factory Method   | Adapter (Class)  | Interpreter             |
 | _Scope_    | _Class_    |                  |                  | Template Method         |
 |------------|------------|------------------|------------------|-------------------------|
 |            | **Objeto** | Abstract Factory | Adapter (Object) | Chain of Responsability |
 |            | _Object_   | Builder          | Bridge           | Command                 |
 |            |            | Prototype        | Composite        | Iterator                |
 |            |            | Singleton        | Decorator        | Mediator                |
 |            |            |                  | Facade           | Memento                 |
 |            |            |                  | Flyweight        | Observer                |
 |            |            |                  | Proxy            | State                   |
 |            |            |                  |                  | Strategy                |
 |            |            |                  |                  | Visitor                 |

Classificação segundo _Metsker_:

| **Intenção**        | **Padrões**                                                              |
|---------------------|--------------------------------------------------------------------------|
| 1. Interfaces       | Adapter, Facade, Composite, Bridge                                       |
| 2. Responsabilidade | Singleton, Observer, Mediator, Proxy, Chain of Responsibility, Flyweight |
| 3. Construção       | Builder, Factory Method, Abstract Factory, Prototype, Memento            |
| 4. Operações        | Template Method, State, Strategy, Command, Interpreter                   |
| 5. Extensões        | Decorator, Iterator, Visitor                                             |

Relacionamento entre padrões:

![Relacionamento entre padrões](../images/arquitetura-gof-relationships.png "Relacionamento entre padrões")

## Padrões

### Strategy

O padrão _Strategy_ define uma família de algoritmos, encapsula cada uma delas e torná-las intercambiáveis. _Strategy_ permite que o algoritmo varie independentemente dos clientes que o utilizam.

Do GoF:
> _Define a family of algorithms, encapsulate each one, and make them interchangeable. Strategy lets the algorithm vary independently from clients that use it._

### Observer

O padrão _Observer_ define uma dependência um-para-muitos entre objetos, de maneira que quando um objeto muda de estado todos os seus dependentes são notificados e atualizados automaticamente.

Do GoF:
> _Define a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically._
