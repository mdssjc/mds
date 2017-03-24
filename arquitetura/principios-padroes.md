# Princípios e Padrões

Os princípios e padrões são as bagagens de experiências do desenvolvedor sobre a etapa de Arquitetura, enquanto os princípios trazem as sugestões e recomendações de expressões idiomáticas para a criação do _software_, os padrões trazem a formalização dos princípios em pares de problema/solução para serem aplicados e moldados aos contextos de _software_.

Os mais utilizados/aplicados são:

* [GRASP](/arquitetura/grasp.md) \(Princípios\)
* [SOLID](/arquitetura/solid.md) \(Princípios de Projeto\)
* [GoF](/arquitetura/gof.md) \(Padrões de Projeto\)
* POSA \(Padrões de Arquitetura\)

## Outros

* **Encapsulamento** \(_Encapsulation_\): é o processo de envolver elementos de programação em entidades abstratas, com o objetivo de proteger a informação de ser utilizada incorretamente, assim separando o tipo de sua classe, ou seja, os dados de seu comportamento ou também o que fazer de como fazer - outros nomes utilizados são Ocultamento de Informação \(_Information Hiding_\) ou Separação de Interesse \(_Separation of Concerns_\). Em projetos, o **Encapsulamento refere-se a API**, enquando o **Ocultamento de Informação a sua implementação**.

* [_**DRY**_](http://c2.com/cgi/wiki?DontRepeatYourself "Dont Repeat Yourself") (_Don’t Repeat Yourself_) / _**WET**_ (_Write Every Time_): princípio sobre o problema da duplicação de conhecimento.

  Cada parte do conhecimento deve ter uma representação única, não ambígua e definitva dentro do sistema.

  Evite código duplicado por abstrair as coisas que são comuns e colocando essas coisas em um único local.

  Tenha cada peça de informação e comportamento em seu sistema em um único e sensível local.

* [_**Execute Around Method**_](http://c2.com/cgi/wiki?ExecuteAroundMethod "Execute Around Method"): controle sobr  e recursos externos, como operações em _cleanup_ e _locks_.

* **Programe para uma interface, não para uma implementação** - _Program to an interface, not to an implementation_: introduzido no livro do GoF, recomenda o uso de abstrações como ponto de acesso entre elementos de programação.

* [**Princípio de _Hollywood_**](http://wiki.c2.com/?HollywoodPrinciple) - _Hollywood Principle_: Não nos chame, nós chamaremos você - _Don't call us, we will call you_, especifica como componentes de alto e baixo nível interagem sem criar dependências.

* [**Ordene, não peça!**](http://wiki.c2.com/?TellDontAsk) - _Tell, dont' ask!_: não peça o produto da informação ao elemento de programação na qual é dono da informação - reduza os acoplamentos.

### Princípios do Desenvolvimento de Pacotes

Os princípios do desenvolvimento de pacotes são apresentados no livro _Agile Software Development - Principles, Patterns, and Practices_ do autor _Robert C. Martin_ \(_Uncle Bob_\), sendo composto por 6 princípios:

#### Granularidade

* [**Princípio da Equivalência entre Liberação e Reuso**](http://wiki.c2.com/?ReuseReleaseEquivalencePrinciple) - _The Reuse-Release Equivalence Principle_ (REP): _the granule of reuse is the granule of release_.

  Adaptado para o livro: a granularidade do reuso é a granularidade do lançamento.

* [**Princípio do Reuso Comum**](http://wiki.c2.com/?CommonReusePrinciple) - _The Commom-Reuse Principle_ (CRP): _the classes in a package are reused together. If you reuse one of the classes in a package, you reuse them all_.

  Adaptado para o livro: as classes em um pacote são todas reutilizadas juntas. Se você reusa uma classe no pacote, reusará todas elas.

* [**Princípio do Fechamento Comum**](http://wiki.c2.com/?CommonClosurePrinciple) - _The Commom-Closure Principle_ (CCP): _the classes in a package should be closed together against the same kinds of changes. A change that affects a package affects all the classes in that package and no other packages_.

  Adaptado para o livro: as classes em um pacote devem ser fechadas em conjunto contra os mesmos tipos de alterações. Uma alteração que afeta um pacote afeta todas as classes nesse pacote e nenhuma em outro pacote.

#### Estabilidade

* [**Princípio das Dependências Acíclicas**](http://wiki.c2.com/?AcyclicDependenciesPrinciple) - _The Acyclic-Dependencies Principle_ (ADP): _allow no cycles in the package-dependency graph_.

  Adaptado para o livro: não permitir ciclos no grafo pacote-dependência.

* [**Princípio das Dependências Estáveis**](http://wiki.c2.com/?StableDependenciesPrinciple) - _The Stable-Dependencies Principle_ (SDP): _depend in the direction of stability_.

  Adaptado para o livro: dependa na direção da estabilidade.
  
  A estabilidade de um pacote dá-se pela relação entre os acoplamentos aferentes (_Afferent Couplings_ - Ca, saídas) e eferentes (_Efferent Couplings_ - Ce, entradas) na formula: **I = Ce / (Ce + Ca)**, sendo estável quando próximo de 0.0 e instável próximo de 1.0.

* [**Princípio das Abstrações Estáveis**](http://wiki.c2.com/?StableAbstractionsPrinciple) - _The Stable-Abstractions Principle_ (SAP): _a package should be as abstract as it is stable_.

  Adaptado para o livro: um pacote deve ser tão abstrato quanto estável.
