# SOLID

O acrônimo _SOLID_ é apresentado no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ \(_Uncle Bob_\), sendo composto por 5 princípios de projeto para o gerenciamento de dependências:

* [**Princípio da Responsabilidade Única**](http://c2.com/cgi/wiki?SingleResponsibilityPrinciple "Single Responsibility Principle") - _Single Responsibility Principle_ \(_SRP_\) por _Robert C. Martin_: todo elemento de programação deve ter uma, e apenas uma razão para mudar - mantenha um equilíbrio entre baixo acoplamento e alta coesão.

  O princípio refere-se as mudanças das funcionalidades por um particular ator da aplicação e não na transformação de uma arquitetura monolítica, principalmente em diversos elementos anêmicos \(uso estrutural sem utilizar de sua principal proposta\).

  O gerenciamento de dependências utiliza-se das caracteristícas de organização da tecnologia utilizada, tais como módulos, pacotes, classes, métodos, funções e etc...

  Aplicar o princípio muito cedo na camada de domínio pode resultar em futuros problemas de projeto.

  Veja também [_Low Coupling_](/arquitetura/grasp.md) e _[High Cohesion](/arquitetura/grasp.md)_ em _GRASP_.

* [**Princípio do Aberto-Fechado**](http://c2.com/cgi/wiki?OpenClosedPrinciple "Open Closed Principle") - _Open-Closed Principle_ \(_OCP_\) por _Bertrand Meyer_ \(criador da linguagem de programação _Eiffel_\) em 1988: projete elementos de programação para serem abertas para extensão, mas fechadas para modificações, minimize as necessidades de fazer mudanças para elementos de programação existentes.

  _Open_: abstração por polimorfismo \/ _Closed_: definição de API.

  O gerenciamento de dependências utiliza-se da abstração para adicionar novas funcionalidades.

  Pode ser aplicado para qualquer elemento de programação.

  Veja também [_Protected Variations_](/arquitetura/grasp.md) em _GRASP_.

* [**Princípio de Substituição de Liskov**](http://c2.com/cgi/wiki?LiskovSubstitutionPrinciple "Liskov Substitution Principle") - _Liskov Substitution Principle_ \(_LSP_\) por _Barbara Liskov_ em 1988: os subtipos devem ser substituídos por seus tipos base.

  Regras sobre o uso do polimorfismo por subtipos de herança, com requisitos de assinatura: contravariância, covariância e exceção; e requisitos de comportamento: invariante, pré-condição e pós-condição.

  Dois problemas comuns são: primeiro, qualquer modificação na classe base afeta todas as classes derivadas; e segundo, as classes derivadas evoluem com proposta diferente da classe base.

  A violação do princípio pode ser corrigida com uso do polimorfismo por subtipos de interface, como relacionamento por composição\/agregação e delegação.

  Veja também _[Polymorphism](/arquitetura/grasp.md)_ em _GRASP_.

* [**Princípio da Segregação de Interfaces**](http://c2.com/cgi/wiki?InterfaceSegregationPrinciple "Interface Segregation Principle") - _Interface Segregation Principle_ \(_ISP_\): os clientes não devem serem forçados a dependerem de métodos que não usam.

* [**Princípio da Inversão de Dependência**](http://c2.com/cgi/wiki?DependencyInversionPrinciple "Dependency Inversion Principle") - _Dependency Inversion Principle_ \(_DIP_\): os módulos de alto nível não devem depender de módulos de baixo nível, ambos devem depender de abstrações.


