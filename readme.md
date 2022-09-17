# LIVRO DO MDS

A ideia desse projeto vem dos livros _Pragmatic Thinking and Learning - Refactor Your "Wetware"_ do autor _Andy Hunt_ e _The Pragmatic Programmer: From Journeyman to Master_ dos autores _Andrew Hunt and David Thomas_, em que aconselha a criação de uma forma de cérebro externo para o registro dos estudos.

O projeto tem a composição de:

![Composição do Projeto](./assets/introduction-project-composition.png 'Composição do Projeto')

- [o livro](https://github.com/mdssjc/mds/ 'o livro') (atemporal);
- [a página](https://marcelo-mds.dev/ 'a página') (temporal);
- [as notas](https://github.com/mdssjc/mds-notes/ 'as notas') (fragmentos); e
- [o repositório](https://github.com/mdssjc/ 'o repositório') (construção).

## Objetivos

Reunir/compilar os conhecimentos/sabedorias utilizados pela profissão de _Craftsman_ - Construtor de _Software_.

## Introdução

Os temas serão pragmaticamente voltados para a construção de _softwares_ na categoria de aplicações, com foco na linguagem ??? (ver observações).

Os capítulos descrevem as etapas marco de um fluxo de desenvolvimento de _software_, considerando uma base sólida como também os aspectos filosóficos e científicos do processo.

O livro é um guia para carregar durante a carreira de construtor de _software_ ou _Craftman_.

### Fluxo de Desenvolvimento

![Fluxo de Desenvolvimento](./assets/introduction-development-flow.png 'Fluxo de Desenvolvimento')

### Linguagens de Programação

As tecnologias para a construção de _software_ são divididas em: _mainstream_ e acadêmica, sendo:

- **mainstream**: tais como _Java_, _.NET_, _C++_, _JavaScript_, _Python_, dentre outras..., ditam o mercado de desenvolvimento de _software_ com uma grande variedade de plataformas e ferramentas (_tooling_), voltadas para os requisitos de desempenho e adaptação para as máquinas atuais, possuem uma grande comunidade impulsionada por evangelistas e entusiastas - geralmente utilizadas para a resolução de problemas.

- **acadêmicas**: tais como _C_, _OCaml_, _Racket_, _Haskell_, dentre outras..., ditam a evolução da tecnologia e possuem uma comunidade especializada e voltada a aprendizagem - geralmente utilizadas para a prototipação, prova de conceito e experimentação de ideias.

**Observação**: existem também as linguagens modernas, tais como: _V_, _Red_, _Zig_, _Roc_, dentre outras..., ditam novas formas de abordagem para os problemas do mercado, pode-se considerar como uma aposta.

### Filosofia

A filosofia da construção de _software_ é composta por TDD, BDD e DDD, sendo:

- **Desenvolvimento Guiado por Testes** - _Test Driven Development_ (TDD): é uma técnica de desenvolvimento de _software_ da Programação Extrema - _Extreme Programming_ (XP), em que os testes são criados antes do código de produção em um ciclo de falhar o teste - passar o teste - refatorar;

- **Desenvolvimento Guiado por Comportamento** - _Behavior Driven Development_ (BDD): é uma técnica de desenvolvimento de _software_ derivada do Desenvolvimento Guiado por Testes - _Test Driven Development_ (TDD) e combinada com práticas do Projeto Orientado a Domínio - _Domain Driven Design_ (DDD) e Análise e Projeto Orientado a Objeto - _Object-Oriented Analysis and Design_ (OOAD), em que utiliza a linguagem do domínio e os testes são criados em paralelo ao código de produção; e

- **Projeto Orientado a Domínio** - _Domain Driven Design_ (DDD): aborda um compilado de experiências aplicadas ao desenvolvimento de _software_.

Essas ideias são aplicadas como base para as modernas arquiteturas baseadas no _Ports-And-Adapters_, tais como: _Hexagonal_, _Onion_ e _Clean Architecture_.

### Ciência

A ciência da construção de _software_ é composta por:

- **Programação Funcional**: paradigma de programação baseado em princípios matemáticos, em que busca declarar as funcionalidades do _software_.

- **Clean Design**: metodologia apresentada por práticas, princípios e padrões aplicados ao _Circle of Life_ da Programação Extrema - _Extreme Programming_ (XP) através das experiências do autor _Robert Cecil Martin_ - conhecido por _Uncle Bob_;

- **Visão 4+1**: modelagem das visões da arquitetura de _software_ em Análise e Projeto Orientado a Objeto - _Object-Oriented Analysis and Design_ (OOAD) na Linguagem de Modelagem Unificada - _Unified Modeling Language_ (UML) com aspectos científicos - definida por _Philippe Kruchten_ no artigo _Architectural Blueprints - The "4+1" View Model of Software Architecture_ em 1995;

- **Effective**: documentação explanado o que fazer e não fazer com a tecnologia na visão dos desenvolvedores com expertise; e

- **Documentação**: documentação e/ou guias sobre o ecossistema da tecnologia na visão dos desenvolvedores.

## Capítulos

- [Introdução](readme.md 'Introdução')
- [Requisitos](requirements/readme.md 'Requisitos')
- Arquitetura
- [Testes](testing/readme.md 'Testes')
- [Código](coding/readme.md 'Código')
- Metodologia
- [Referências](references.md 'Referências')

## Observação

Para visualizar a versão antiga do livro, acesse a `branch old`.

A linguagem de exemplo do livro não está definida, podendo ser o _Scala_ ou _OCaml/Racket_ (utilizado por [Dan Grossman](https://homes.cs.washington.edu/~djg/ 'Dan Grossman')). Existe também a possibilidade do uso dessas linguagens com uma implementação final em _Java_ ou _Dart_.

## Data da Atualização

30/09/2022
