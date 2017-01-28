# SOLID

O acrônimo _SOLID_ é apresentado no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ \(_Uncle Bob_\), sendo composto por 5 princípios de projeto para o gerenciamento de dependências:

* [**Princípio da Responsabilidade Única**](http://c2.com/cgi/wiki?SingleResponsibilityPrinciple "Single Responsibility Principle") - _Single Responsibility Principle_ \(_SRP_\) por _Robert C. Martin_ com base nos trabalhos de _Tom DeMarco_ e _Meilir Page-Jones_ sobre coesão:

  **"_A class should have only one reason to change_"**

  Adaptado para o livro: _Um elemento de programação deve ter apenas uma razão para mudar_ - mantenha um equilíbrio entre baixo acoplamento e alta coesão.

  O princípio refere-se as mudanças das funcionalidades por um particular ator da aplicação e não na transformação de uma arquitetura monolítica, principalmente em diversos elementos anêmicos \(uso estrutural sem utilizar de sua principal proposta\).

  O gerenciamento de dependências utiliza-se das características de organização da tecnologia utilizada, tais como módulos, pacotes, classes, métodos, funções e etc...

  Aplicar o princípio muito cedo na camada de domínio pode resultar em futuros problemas de projeto.

  Veja também [_Low Coupling_](/arquitetura/grasp.md) e [_High Cohesion_](/arquitetura/grasp.md) em _GRASP_.

* [**Princípio do Aberto-Fechado**](http://c2.com/cgi/wiki?OpenClosedPrinciple "Open Closed Principle") - _Open-Closed Principle_ \(_OCP_\) por _Bertrand Meyer_ \(criador da linguagem de programação _Eiffel_\) em 1988:

  **"_Software entities \(classes, modules, functions, etc.\) should be open for extension, but closed for modification_"**

  Adaptado para o livro: _Os elementos de programação deve ser aberto para a extensão, mas fechado para modificação_ - minimize as necessidades de fazer mudanças para elementos de programação existentes.

  _Open_: abstração por polimorfismo / _Closed_: definição de API.

  O gerenciamento de dependências utiliza-se da abstração para adicionar novas funcionalidades, assim mantendo a definição sem alterações.

  Pode ser aplicado para qualquer elemento de programação.

  Veja também [_Protected Variations_](/arquitetura/grasp.md) em _GRASP_.

* [**Princípio de Substituição de Liskov**](http://c2.com/cgi/wiki?LiskovSubstitutionPrinciple "Liskov Substitution Principle") - _Liskov Substitution Principle_ \(_LSP_\) por _Barbara Liskov_ em 1988:

  **"_Subtypes must be substitutable for their base types_"**

  Adaptado para o livro: _Os subtipos devem ser substituíveis pelos seus tipos de base_.

  Definição do princípio:

  > _If for each object o1 of type S there is an object o2 of type T such that for all programs P defined in terms of T, the behavior of P is unchanged when o1 is substituted for o2 then S is a subtype of T_
  >
  > _Se para cada objeto o1 do tipo S há um objeto o2 do tipo T de forma que, para todos os programas P definidos em termos de T, o comportamento de P é inalterado quando o1 é substituído por o2 então S é um subtipo de T_

  Regras sobre o uso do polimorfismo por subtipos de herança são baseados no trabalho _Design By Contract_ \(_DBC_\) de _Bertrand Meyer_,

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

  A violação do princípio pode ser corrigida com uso do polimorfismo por subtipos de interface, como relacionamento por composição/agregação e delegação.

  Veja também [_Polymorphism_](/arquitetura/grasp.md) em _GRASP_.

* [**Princípio da Segregação de Interfaces**](http://c2.com/cgi/wiki?InterfaceSegregationPrinciple "Interface Segregation Principle") - _Interface Segregation Principle_ \(_ISP_\):

  **"_Clients should not be forced to depend on methods that they do not use_"**

  Adaptado para o livro: _Os clientes não devem serem forçados a dependerem de métodos que não usam_.

* [**Princípio da Inversão de Dependência**](http://c2.com/cgi/wiki?DependencyInversionPrinciple "Dependency Inversion Principle") - _Dependency Inversion Principle_ \(_DIP_\):

  Definição do princípio:

  > a. High-level modules should not depend on low-level modules. Both should depend on abstractions.
  >
  > b. Abstractions should not depend on details. Details should depend on abstractions.
  >
  > a. Os módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações.
  >
  > b. Abstrações não devem depender de detalhes. Detalhes devem depender de abstrações.

  Também conhecido por Princípio de _Hollywood_: "Não nos chame, nós chamaremos você" - "_Don't call us, we'll call you_".
