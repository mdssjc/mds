# Arquitetura

A arquitetura do _software_ consiste de:

* [**Cenário**](/arquitetura/cenario.md): Descrevendo o problema.
* [**Análise**](/arquitetura/analise.md): O que fazer para solucionar o problema? 
* **[Projeto](arquitetura/projeto.md)**: Como fazer para solucionar o problema? 

## Padrões

Os padrões são experiências compartilhadas de desenvolvedores experientes sobre a modelagem e codificação de _software_.

### Básico OO

* Encapsulamento
* Interface
* Delegação

### GRASP

O acrônimo _GRASP_ - General Responsibility Assignment Software Patterns apresentado no livro _Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development_ \(_3rd Edition_\) do autor _Craig Larman_ explana os princípios fundamentais da subetapa de Projeto em modelos UML e CRC _Cards_, composto por 9 princípios \(5 básicos e 4 avançados\):

* **Criador** - _Creator_: atribuição da responsabilidade \(fazer\) de criação ao elemento de programação. Problema: Quem cria um A? Solução: Abribua a B a responsabilidade de criar uma instância de A, se:

  * B contém ou agrega A.
  * B registra ou guarda instância de A.
  * B faz uso de A.
  * B tem dados de inicialização de A.

* **Especialista na Informação** - _Information Expert_ \(_Expert_\): atribuição da responsabilidade \(saber e fazer\) ao elemento de programação com a informação.
  Problema: Qual é o princípio fundamental para atribuir responsabilidades aos elementos?
  Solução: Atribua uma responsabilidade para o elemento que tem a informação necessária para cumpri-la.

* **Baixo Acoplamento** - _Low Coupling_: reduzação das dependências por manter alta coesão nas responsabilidades;
* **Alta Coesão** - _High Cohesion_: medida do grau de relacionamento das responsabilidades com a tarefa\/descrição do elemento de programação em questão;
* **Controlador** - _Controller_: também conhecido por Coordenadora, elemento reponsável por manipular os eventos no sistema, quando centralizado é conhecido por Controlador de Fachada - _Front Controller_ e quando implementa a lógica da aplicação é conhecido por Controlador de Caso de Uso ou de Sessão - _Controller_;

* **Poliformismo** - _Polymorphism_: _em edição_;

* **Indireção** - _Indirection_: _em edição_;

* **Fabricação\/Invenção Pura** - _Pure Fabrication_: _em edição_; e

* **Variações Protegidas** - _Protected Variations_: _em edição._


### SOLID

O acrônimo _SOLID_ apresentado no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ \(_Uncle Bob_\), composto por 5 princípios de projeto de classes:

* **[Princípio da Responsabilidade Única](http://c2.com/cgi/wiki?SingleResponsibilityPrinciple "Single Responsibility Principle")** - _Single Responsibility Principle_ \(_SRP_\) por _Robert C. Martin_: todo módulo ou classe deve ter uma, e apenas uma razão para mudar - mantenha um equilíbrio entre baixo acoplamento e alta coesão;

  O princípio refere-se as mudanças das funcionalidades por um particular ator da aplicação e não na transformação de uma arquitetura monolítica, principalmente em diversas classes anêmicas.

  Aplicar o princípio muito cedo na camada de domínio pode resultar em futuros problemas de projeto.

* **[Princípio do Aberto-Fechado](http://c2.com/cgi/wiki?OpenClosedPrinciple "Open Closed Principle")** - _Open-Closed Principle_ \(_OCP_\) por _Bertrand Meyer_ ~~em 1988~~: projete classes para serem abertas para extensão mas fechadas para modificações, minimize as necessidades para fazer mudanças para classes existentes;

* [**Princípio de Substituição de Liskov**](http://c2.com/cgi/wiki?LiskovSubstitutionPrinciple "Liskov Substitution Principle") - _Liskov Substitution Principle_ \(_LSP_\) por _Barbara Liskov_ em

  1988: os subtipos devem ser substituidos por seus tipos base;


* [**Princípio da Segregação de Interfaces**](http://c2.com/cgi/wiki?InterfaceSegregationPrinciple "Interface Segregation Principle") - _Interface Segregation Principle_ \(_ISP_\): os clientes não devem serem forçados a dependerem de métodos que não usam; e

* **[Princípio da Inversão de Dependência](http://c2.com/cgi/wiki?DependencyInversionPrinciple "Dependency Inversion Principle")** - _Dependency Inversion Principle_ \(_DIP_\): os módulos de alto nível não devem depender de módulos de baixo nível, ambos devem depender de abstrações;


### GoF

### POSA

### Outros

* [**_DRY_**](http://c2.com/cgi/wiki?DontRepeatYourself "Dont Repeat Yourself") \(_Don’t Repeat Yourself_\) \/ **_WET_** \(_Write Every Time_\): princípio sobre o problema da duplicação de código.
* **_[Execute Around Method](http://c2.com/cgi/wiki?ExecuteAroundMethod "Execute Around Method")_**: controle sobre recursos externos, como operações em _cleanup_ e _locks_.

