# SOLID

O acrônimo _SOLID_ é apresentado no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ (_Uncle Bob_), sendo composto por 5 princípios de projeto para o gerenciamento de dependências.

Os sintomas (_design smells_) de um projeto ruim são:
* **Rigidez** - _Rigidity_: o projeto é difícil de mudar;
* **Fragilidade** - _Fragility_: o projeto é fácil de quebrar;
* **Imobilidade** - _Immobility_: o projeto é difícil de reusar;
* **Viscosidade** - _Viscosity_: é difícil fazer a coisa certa;
* **Complexidade Desnecessária** - _Needless Complexity_: sobreprojeto, excesso de complexidade adicional;
* **Repetição Desnecessária** - _Needless Repetition_: abuso do _mouse_, excesso de repetição; e
* **Opacidade** - _Opacity_: expressão desorganizada.

---

* [**Princípio da Responsabilidade Única**](http://c2.com/cgi/wiki?SingleResponsibilityPrinciple "Single Responsibility Principle") - _Single Responsibility Principle_ (SRP) por _Robert C. Martin_ com base nos trabalhos de _Tom DeMarco_ e _Meilir Page-Jones_ sobre coesão:

  **"_A class should have only one reason to change_"**

  Adaptado para o livro: _Um elemento de programação deve ter apenas uma razão para mudar_ - mantenha um equilíbrio entre baixo acoplamento e alta coesão.

  O princípio refere-se as mudanças das funcionalidades por um particular ator da aplicação e não na transformação de uma arquitetura monolítica, principalmente em diversos elementos anêmicos (uso estrutural sem utilizar de sua principal proposta).

  O gerenciamento de dependências utiliza-se das características de organização da tecnologia utilizada, tais como módulos, pacotes, classes, métodos, funções e etc...

  Aplicar o princípio muito cedo na camada de domínio pode resultar em futuros problemas de projeto.

  Veja também [_Low Coupling_](/arquitetura/grasp.md) e [_High Cohesion_](/arquitetura/grasp.md) em _GRASP_.

* [**Princípio do Aberto-Fechado**](http://c2.com/cgi/wiki?OpenClosedPrinciple "Open Closed Principle") - _Open-Closed Principle_ (OCP) por _Bertrand Meyer_ (criador da linguagem de programação _Eiffel_) em 1988:

  **"_Software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification_"**

  Adaptado para o livro: _Os elementos de programação deve ser aberto para a extensão, mas fechado para modificação_ - minimize as necessidades de fazer mudanças para elementos de programação existentes.

  _Open_: abstração por polimorfismo / _Closed_: definição de Interface de Programação de Aplicação - _Application Programming Interface_ (API).

  O gerenciamento de dependências utiliza-se da abstração e polimorfismo para adicionar novas funcionalidades, assim mantendo a definição sem alterações.

  Pode ser aplicado para qualquer elemento de programação.

  Veja também [_Protected Variations_](/arquitetura/grasp.md) em _GRASP_.

* [**Princípio de Substituição de Liskov**](http://c2.com/cgi/wiki?LiskovSubstitutionPrinciple "Liskov Substitution Principle") - _Liskov Substitution Principle_ (LSP) por _Barbara Liskov_ em 1988:

  **"_Subtypes must be substitutable for their base types_"**

  Adaptado para o livro: _Os subtipos devem ser substituíveis pelos seus tipos de base_.

  Definição do princípio:

  > _If for each object o1 of type S there is an object o2 of type T such that for all programs P defined in terms of T, the behavior of P is unchanged when o1 is substituted for o2 then S is a subtype of T_
  >
  > _Se para cada objeto o1 do tipo S há um objeto o2 do tipo T de forma que, para todos os programas P definidos em termos de T, o comportamento de P é inalterado quando o1 é substituído por o2 então S é um subtipo de T_

  Regras sobre o uso do polimorfismo por subtipos de herança são baseados no trabalho _Design By Contract_ (DBC) de _Bertrand Meyer_,

  com requisitos de assinatura:

  * contravariância: dos argumentos/parâmetros das funções/métodos em um subtipo, sendo o sentido do relacionamento ascendente ao tipo, ou seja, assume um tipo menos específico;
  * covariância: dos tipos de retorno em um subtipo, sendo o sentido do relacionamento descendente ao tipo, ou seja, assume um tipo mais específico; e
  * exceção: não pode ser novas e/ou maior que a definida no tipo.

  e requisitos de comportamento:

  * invariante: qualquer predicado deve ser preservado em um subtipo;
  * pré-condição: uma condição ou predicado não pode ser mais forte em um subtipo, porém pode ser mais fraca; e
  * pós-condição: uma condição ou predicado não pode ser mais fraca em um subtipo, porém pode ser mais forte.

  Dois problemas comuns são: primeiro, qualquer modificação no tipo afeta todos os subtipos; e segundo, os subtipos evoluem com proposta diferente do tipo.

  O gerenciamento de dependências utiliza-se do polimorfismo para manter correta a árvore de relacionamentos.
  
  Uma violação do princípio é uma violação latente do OCP.

  A violação do princípio pode ser corrigida com uso do polimorfismo por subtipos de interface, como relacionamento por composição/agregação e delegação.

  Veja também [_Polymorphism_](/arquitetura/grasp.md) em _GRASP_.

* [**Princípio da Segregação de Interfaces**](http://c2.com/cgi/wiki?InterfaceSegregationPrinciple "Interface Segregation Principle") - _Interface Segregation Principle_ (ISP):

  **"_Clients should not be forced to depend on methods that they do not use_"**

  Adaptado para o livro: _Os clientes não devem serem forçados a dependerem de métodos que não usam_.

* [**Princípio da Inversão de Dependência**](http://c2.com/cgi/wiki?DependencyInversionPrinciple "Dependency Inversion Principle") - _Dependency Inversion Principle_ (DIP):

  Definição do princípio:

  > a. High-level modules should not depend on low-level modules. Both should depend on abstractions.
  >
  > b. Abstractions should not depend on details. Details should depend on abstractions.
  >
  > a. Os módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações.
  >
  > b. Abstrações não devem depender de detalhes. Detalhes devem depender de abstrações.

  Também conhecido por Princípio de _Hollywood_: "Não nos chame, nós chamaremos você" - "_Don't call us, we'll call you_".
  
  Solução para dependências: cíclica e estável-instável/flexível.

---

## Princípios do Desenvolvimento de Pacotes

Os princípios do desenvolvimento de pacotes são apresentados no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ (_Uncle Bob_), sendo composto por 6 princípios:

### Granularidade: Os Princípios da Coesão de Pacotes

* [**Princípio da Equivalência entre Liberação e Reuso**](http://wiki.c2.com/?ReuseReleaseEquivalencePrinciple) - _The Reuse-Release Equivalence Principle_ (REP): _the granule of reuse is the granule of release_.

  Adaptado para o livro: a granularidade do reuso é a granularidade do lançamento.

  _Ou todas as classes em um pacote são reutilizáveis ou nenhuma delas são._

* [**Princípio do Reuso Comum**](http://wiki.c2.com/?CommonReusePrinciple) - _The Commom-Reuse Principle_ (CRP): _the classes in a package are reused together. If you reuse one of the classes in a package, you reuse them all_.

  Adaptado para o livro: as classes em um pacote são todas reutilizadas juntas. Se você reusa uma classe no pacote, reusará todas elas.

* [**Princípio do Fechamento Comum**](http://wiki.c2.com/?CommonClosurePrinciple) - _The Commom-Closure Principle_ (CCP): _the classes in a package should be closed together against the same kinds of changes. A change that affects a package affects all the classes in that package and no other packages_.

  Adaptado para o livro: as classes em um pacote devem ser fechadas em conjunto contra os mesmos tipos de alterações. Uma alteração que afeta um pacote afeta todas as classes nesse pacote e nenhuma em outro pacote.

### Estabilidade: Os Princípios do Acoplamento de Pacotes

* [**Princípio das Dependências Acíclicas**](http://wiki.c2.com/?AcyclicDependenciesPrinciple) - _The Acyclic-Dependencies Principle_ (ADP): _allow no cycles in the package-dependency graph_.

  Adaptado para o livro: não permitir ciclos no grafo pacote-dependência.

* [**Princípio das Dependências Estáveis**](http://wiki.c2.com/?StableDependenciesPrinciple) - _The Stable-Dependencies Principle_ (SDP): _depend in the direction of stability_.

  Adaptado para o livro: dependa na direção da estabilidade.
  
  A estabilidade de um pacote dá-se pela relação dos acoplamentos aferentes (_Afferent Couplings_ - Ca, saídas) pelos acoplamentos eferentes (_Efferent Couplings_ - Ce, entradas) na formula: **I = Ce / (Ce + Ca)**, sendo estável quanto mais próximo de 0.0 e instável quanto mais próximo de 1.0.

* [**Princípio das Abstrações Estáveis**](http://wiki.c2.com/?StableAbstractionsPrinciple) - _The Stable-Abstractions Principle_ (SAP): _a package should be as abstract as it is stable_.

  Adaptado para o livro: um pacote deve ser tão abstrato quanto estável.

  A abstração (A) de um pacote dá-se pela relação do número de classes abstratas (Na) pelo número de classes (Nc) na formula: **A = Na / Nc**, sendo não abstrata quanto mais próximo de 0.0 e abstrata quanto mais próximo de 1.0.
