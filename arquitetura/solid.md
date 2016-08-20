# SOLID

O acrônimo _SOLID_ apresentado no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ \(_Uncle Bob_\), composto por 5 princípios de projeto de classes:

* **[Princípio da Responsabilidade Única](http://c2.com/cgi/wiki?SingleResponsibilityPrinciple "Single Responsibility Principle")** - _Single Responsibility Principle_ \(_SRP_\) por _Robert C. Martin_: todo módulo ou classe deve ter uma, e apenas uma razão para mudar - mantenha um equilíbrio entre baixo acoplamento e alta coesão;

  O princípio refere-se as mudanças das funcionalidades por um particular ator da aplicação e não na transformação de uma arquitetura monolítica, principalmente em diversas classes anêmicas.

  Aplicar o princípio muito cedo na camada de domínio pode resultar em futuros problemas de projeto.

  Veja também [_High Cohesion_](/arquitetura/grasp.md) em _GRASP_.

* **[Princípio do Aberto-Fechado](http://c2.com/cgi/wiki?OpenClosedPrinciple "Open Closed Principle")** - _Open-Closed Principle_ \(_OCP_\) por _Bertrand Meyer_ em 1988: projete classes para serem abertas para extensão mas fechadas para modificações, minimize as necessidades de fazer mudanças para classes existentes;

  _Open_: poliformismo \/ _Closed_: definição de API.

  Veja também _[Protected Variations](/arquitetura/grasp.md)_ em _GRASP_.

* **[Princípio de Substituição de Liskov](http://c2.com/cgi/wiki?LiskovSubstitutionPrinciple "Liskov Substitution Principle")** - _Liskov Substitution Principle_ \(_LSP_\) por _Barbara Liskov_ em 1988: os subtipos devem ser substituidos por seus tipos base;

  Regras sobre o uso do poliformismo por subtipos de herança, com requisitos de assinatura: contravariância, covariância e exceção; e requisitos de comportamento: invariante, pré-condição e pós-condição.

  A violação do princípio pode ser corrigida com poliformismo por subtipos de interface, como relacionamento por composição e delegação.
  Veja também [_Polymorphism_](/arquitetura/grasp.md) em _GRASP_.

* **[Princípio da Segregação de Interfaces](http://c2.com/cgi/wiki?InterfaceSegregationPrinciple "Interface Segregation Principle")** - _Interface Segregation Principle_ \(_ISP_\): os clientes não devem serem forçados a dependerem de métodos que não usam; e

* **[Princípio da Inversão de Dependência](http://c2.com/cgi/wiki?DependencyInversionPrinciple "Dependency Inversion Principle")** - _Dependency Inversion Principle_ \(_DIP_\): os módulos de alto nível não devem depender de módulos de baixo nível, ambos devem depender de abstrações;


