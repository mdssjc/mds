# Princípios, Padrões e Práticas

Os princípios, padrões e práticas são as bagagens de experiências do desenvolvedor sobre a etapa de Arquitetura - com a adição de _complexidade adicional_ na maioria dos casos: enquanto os princípios trazem as sugestões e recomendações de expressões idiomáticas para a criação do _software_, os padrões trazem a formalização dos princípios em pares de problema/solução para serem aplicados e moldados aos contextos de _software_, por fim as práticas trazem as atividades/técnicas executadas durante o projeto pelo XP, SPD e XDD.

Os problemas são:
```
detectados pelas Práticas,
diagnosticados pelos Príncipios e
solucionados pelos Padrões.
```

Os mais utilizados/aplicados são:

* [Práticas](/arquitetura/praticas.md) (Aplicação do XP, SPD e XDD)
* [Básicos](/arquitetura/basicos.md) (Princípios Básicos)
* [Gerais](/arquitetura/gerais.md) (Princípios Gerais)
* [GRASP](/arquitetura/grasp.md) (Princípios Fundamentais)
* [SOLID](/arquitetura/solid.md) (Princípios de Projeto)
* [GoF](/arquitetura/gof.md) (Padrões de Projeto)
* [POSA](/arquitetura/posa.md) (Padrões de Arquitetura)

## Outros

* **Encapsulamento** - _Encapsulation_: é o processo de envolver elementos de programação em entidades abstratas, com o objetivo de proteger a informação (em meios controlados) de ser utilizada incorretamente, assim separando o tipo de sua classe, ou seja, os dados de seu comportamento ou também o que fazer de como fazer - outros nomes utilizados são Ocultamento de Informação (_Information Hiding_) ou Separação de Interesse (_Separation of Concerns_). Em projetos, o **Encapsulamento refere-se a API**, enquando o **Ocultamento de Informação a sua implementação**.

* [_**DRY**_](http://c2.com/cgi/wiki?DontRepeatYourself "Dont Repeat Yourself") (_Don’t Repeat Yourself_) / _**WET**_ (_Write Every Time_): princípio sobre o problema da duplicação de conhecimento.

  Cada parte do conhecimento deve ter uma representação única, não ambígua e definitva dentro do sistema.

  Evite código duplicado por abstrair as coisas que são comuns e colocando essas coisas em um único local.

  Tenha cada peça de informação e comportamento em seu sistema em um único e sensível local.

* [_**Execute Around Method**_](http://c2.com/cgi/wiki?ExecuteAroundMethod "Execute Around Method"): controle sobr  e recursos externos, como operações em _cleanup_ e _locks_.

* **Programe para uma interface, não para uma implementação** - _Program to an interface, not to an implementation_: introduzido no livro do GoF, recomenda o uso de abstrações como ponto de acesso entre elementos de programação.

* [**Princípio de _Hollywood_**](http://wiki.c2.com/?HollywoodPrinciple) - _Hollywood Principle_: Não nos chame, nós chamaremos você - _Don't call us, we will call you_, especifica como componentes de alto e baixo nível interagem sem criar dependências.

* [**Ordene, não peça!**](http://wiki.c2.com/?TellDontAsk) - _Tell, dont' ask!_: peça o produto da informação ao elemento de programação na qual é dono da informação - reduza os acoplamentos, priorizando o encapsulamento.
