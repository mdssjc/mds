# GoF

O acrônimo GoF - _Gang of Four_ apresentado no livro _Design Patterns_ dos autores _Erich Gamma_,
 _John Vlissides_, _Ralph Jonhson_ e _Richard Helm_ explana um catálogo de 23 genéricas soluções para o desenvolvimento de _software_ no paradigma orientado a objetos.

 Os _Design Patterns_ do livro são: "_descrições de objetos e classes comunicantes que precisam ser personalizadas para resolver um problema geral de projeto num contexto particular_".

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
