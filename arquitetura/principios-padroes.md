# Princípios e Padrões

Os princípios e padrões são as bagagens de experiências do desenvolvedor sobre a etapa de Arquitetura, enquanto os princípios trazem as sugestões e recomendações de expressões idiomáticas para a criação do _software_, os padrões trazem a formalização dos princípios em pares de problema/solução para serem aplicados e moldados aos contextos de _software_.

* [GRASP](/arquitetura/grasp.md)
* [GoF](/arquitetura/gof.md)
* [SOLID](/arquitetura/solid.md)

### Básico

* **Encapsulamento** \(_Encapsulation_\): é o processo de envolver elementos de programação em entidades abstratas, com o objetivo de proteger a informação de ser utilizada incorretamente, assim separando o tipo de sua classe, ou seja, os dados de seu comportamento - outros nomes utilizados são Ocultamento de Informação \(_Information Hiding_\) ou Separação de Interesse \(_Separation of Concerns_\).
* Interface
* Delegação
* ~~Acoplamento~~
* ~~Responsabilidade~~

### GoF

_em edição_

### POSA

_em edição_

### Outros

* [_**DRY**_](http://c2.com/cgi/wiki?DontRepeatYourself "Dont Repeat Yourself") \(_Don’t Repeat Yourself_\) / _**WET**_ \(_Write Every Time_\): princípio sobre o problema da duplicação de código.

  Evite código duplicado por abstrair as coisas que são comuns e colocando essas coisas em um único local.

  Tenha cada peça de informação e comportamento em seu sistema em um único e sensível local.

* [_**Execute Around Method**_](http://c2.com/cgi/wiki?ExecuteAroundMethod "Execute Around Method"): controle sobre recursos externos, como operações em _cleanup_ e _locks_.




