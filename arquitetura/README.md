# Arquitetura

A arquitetura do _software_ consiste de:

* **[Cenário](/arquitetura/cenario.md)**: Descrevendo o problema.
* **[Análise](/arquitetura/analise.md)**: O que fazer para solucionar o problema? 
* [**Projeto**](arquitetura/projeto.md): Como fazer para solucionar o problema? 

## Padrões

### Básico OO

* Encapsulamento
* Interface
* Delegação

### GRASP

O acrônimo _GRASP_ - General Responsibility Assignment Software Patterns apresentado no livro _Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development_ \(_3rd Edition_\) do autor _Craig Larman_, composto por 9 princípios:

* Low Coupling
* High Cohesion
* Especialista de Informação - _Information Expert_: 
* Creator
* Controller
* Polymorphism
* Indirection
* Pure Fabrication
* Protected Variations

### SOLID

O acrônimo _SOLID_ apresentado no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ \(_Uncle Bob_\), composto por 5 princípios de projeto de classes:

* [**Princípio da Responsabilidade Única**](http://c2.com/cgi/wiki?SingleResponsibilityPrinciple "Single Responsibility Principle") - _Single Responsibility Principle_ \(_SRP_\) por _Robert C. Martin_: todo módulo ou classe deve ter uma, e apenas uma razão para mudar - mantenha um equilíbrio entre baixo acoplamento e alta coesão;

  O princípio refere-se as mudanças das funcionalidades por um particular ator da aplicação e não na transformação de uma arquitetura monolítica, principalmente em diversas classes anêmicas.

  Aplicar o princípio muito cedo na camada de domínio pode resultar em futuros problemas de projeto.

* [**Princípio do Aberto-Fechado**](http://c2.com/cgi/wiki?OpenClosedPrinciple "Open Closed Principle") - _Open-Closed Principle_ \(_OCP_\) por _Bertrand Meyer_ ~~em 1988~~: projete classes para serem abertas para extensão mas fechadas para modificações, minimize as necessidades para fazer mudanças para classes existentes;

* **[Princípio de Substituição de Liskov](http://c2.com/cgi/wiki?LiskovSubstitutionPrinciple "Liskov Substitution Principle")** - _Liskov Substitution Principle_ \(_LSP_\) por _Barbara Liskov_ em

  1988: os subtipos devem ser substituidos por seus tipos base;


* **[Princípio da Segregação de Interfaces](http://c2.com/cgi/wiki?InterfaceSegregationPrinciple "Interface Segregation Principle")** - _Interface Segregation Principle_ \(_ISP_\): os clientes não devem serem forçados a dependerem de métodos que não usam; e

* [**Princípio da Inversão de Dependência**](http://c2.com/cgi/wiki?DependencyInversionPrinciple "Dependency Inversion Principle") - _Dependency Inversion Principle_ \(_DIP_\): os módulos de alto nível não devem depender de módulos de baixo nível, ambos devem depender de abstrações;


### GoF

### POSA

### Outros

* _**[DRY](http://c2.com/cgi/wiki?DontRepeatYourself "Dont Repeat Yourself")**_ \(_Don’t Repeat Yourself_\) \/ _**WET**_ \(_Write Every Time_\): princípio sobre o problema da duplicação de código.
* [_**Execute Around Method**_](http://c2.com/cgi/wiki?ExecuteAroundMethod "Execute Around Method"): controle sobre recursos externos, como operações em _cleanup_ e _locks_.

