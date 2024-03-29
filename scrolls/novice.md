# NOVATO

## Práticas

### XP

- **Programação Extrema** - _Extreme Programming_ (XP): estude pela página
  [www.extremeprogramming.org](http://www.extremeprogramming.org 'Extreme
Programming').
- Execução em iteração (como um miniprojeto), assim recebendo constante
  _feedback_ para cada etapa do _software_ em funcionamento.
- Entregue _software_: que seja necessário, no tempo e no orçamento.

### SPD

- **_How to Design Programs_**: estude pelo _ebook online_
  [HtDP2e](http://www.ccs.neu.edu/home/matthias/HtDP2e 'How to Design Programs,
Second Edition');
- **_How to Code: Simple Data_**: estude pelo curso
  [HtC1x](https://www.edx.org/course/how-code-simple-data-ubcx-htc1x 'How to
Code: Simple Data'); e
- **_How to Code: Complex Data_**: estude pelo curso
  [HtC2x](https://www.edx.org/course/how-code-complex-data-ubcx-htc2x 'How to
Code: Complex Data').

### Regra dos três

Aplique os padrões após três diferentes exemplos do mesmo problema no código.

## Princípios

### Gerais

- [**Não se Repita**](http://wiki.c2.com/?DontRepeatYourself "Don't Repeat
Yourself") - _Don’t Repeat Yourself_ (DRY) / _Write Every Time_ (WET):
  princípio sobre o problema da duplicação de conhecimento.

  Cada parte do conhecimento deve ter uma representação única, não ambígua e
  definitiva dentro do sistema.

  Evite código duplicado por abstrair as coisas que são comuns e colocando essas
  coisas em um único local.

  Tenha cada peça de informação e comportamento em seu sistema em um único e
  sensível local.

- [**Execute Around Method**](http://wiki.c2.com/?ExecuteAroundMethod 'Execute
Around Method'): controle sobre recursos externos, como operações em _cleanup_
  e _locks_.

- [**Princípio de Hollywood**](http://wiki.c2.com/?HollywoodPrinciple 'Hollywood Principle') - _Hollywood Principle_: Não nos chame, nós chamaremos
  você - _Don't call us, we will call you_, especifica como componentes de alto
  e baixo nível interagem sem criar dependências, sendo uma técnica para a
  construção de _frameworks_ e componentes.

- [**Ordene, não peça!**](http://wiki.c2.com/?TellDontAsk "Tell, don't ask!") -
  _Tell, don't ask!_: peça o produto da informação ao elemento de programação na
  qual é dono da informação - reduza os acoplamentos, priorizando o
  encapsulamento.

  Técnicas para a refatoração: delegação e redirecionamento.

- [**Princípio do Mínimo Conhecimento**](http://wiki.c2.com/?LawOfDemeter 'Principle of Least Knowledge') - _Principle of Least Knowledge_: também
  conhecido por _Law of Demeter_ (1988) ou _Don't Talk to Strangers_, fale
  somente com seus amigos imediatos:

  1. O elemento em si;
  2. Os elementos passados como parâmetros para o elemento;
  3. Quaisquer elementos criados e/ou instanciados;
  4. Quaisquer componentes do elemento; e
  5. Os elementos globais.

- [**Mantenha Simples, Estúpido**](http://wiki.c2.com/?KeepItSimple 'Keep It
Simple, Stupid') - _Keep It Simple, Stupid_ (KISS): _em edição_.

- [**Você Não Vai Precisar Disso**](http://wiki.c2.com/?YouArentGonnaNeedIt "You
Aren't Gonna Need It") - _You Aren't Gonna Need It_ (YAGNI): resista a
  urgência da necessidade no futuro, guiando o desenvolvimento através do TDD.

### Conceitos

- **Herança** - _Inheritance_: é o ato de um elemento de programação estender as
  responsabilidades de outro elemento de programação através da construção de um
  novo nível na hierarquia durante o tempo de compilação.

- [**Encapsulamento**](http://wiki.c2.com/?EncapsulationDefinition 'Encapsulation') - _Encapsulation_: é o processo de envolver elementos de
  programação em entidades maiores e mais abstratas, com o objetivo de proteger
  a informação (em meios controlados) de ser utilizada incorretamente, assim
  separando o tipo de sua classe, ou seja, os dados de seu comportamento ou
  também o que fazer de como fazer - outros nomes utilizados são Ocultamento de
  Informação (_Information Hiding_) ou Separação de Interesse (_Separation of
  Concerns_). Em projetos, o **Encapsulamento refere-se a API**, enquando o
  **Ocultamento de Informação a sua implementação**.

  Separa o que varia do que permanece constante.

  Protege os elementos de programação de desnecessárias mudanças.

- [**Polimorfismo**](http://wiki.c2.com/?PolyMorphism 'Polimorfismo')-
  _Polymorphism_: _em edição_.

- **Delegação** - _Delegation_: é o ato de um elemento de programação encaminhar
  uma necessidade/responsabilidade para outro elemento de programação, para ser
  executado em função do primeiro.

  Blinda seus elementos de programação de alterações nos outros elementos de
  programação.

  É um exemplo extremo de composição.

- **Redirecionamento** - _Forwarding_: _em edição_.

- **Composição** - _Composition_: é o ato de um elemento de programação usar as
  funcionalidades/comportamentos de uma família de outros elementos de
  programação e modificar (por seleção) essas funcionalidades/comportamentos em
  tempo de execução.

- **Agregação** - _Aggregation_: é o ato de um elemento de programação usar as
  funcionalidades/comportamentos de outros elementos de programação, mas sem
  controlar seu tempo de vida.

- **Associação** - _Acquaintance_: _em edição_.
