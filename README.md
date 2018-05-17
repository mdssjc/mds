# Introdução

Este livro tem como objetivo reunir/compilar os fragmentos de
conhecimento/sabedoria utilizados pela profissão de _Craftsman_ - **Construtor
de Software**.

Os temas serão pragmaticamente voltados para o ramo Sistema de Computação,
principalmente abordando a disciplina de **Arquitetura de Software e Testes**
com Algoritmos e Mineração de Dados com foco nos dialetos da tecnologia _Lisp_.

Os capítulos descrevem as etapas marco de um fluxo de desenvolvimento de
_software_, considerando uma base sólida como também os aspectos filosóficos e
científicos do processo.

## A Base

As tecnologias para a construção de _software_ são divididas em: _mainstream_ e
acadêmica.

As tecnologias _mainstream_, tais como _Java_, _.NET_, _C++_, _JavaScript_,
_Python_, dentre outras..., ditam o mercado de desenvolvimento de _software_ com
uma grande variedade de plataformas e ferramentas (_tooling_), voltadas para os
requisitos de desempenho e adaptação para as máquinas atuais - são as linguagens
primárias, geralmente utilizadas para a resolução de problemas.

As tecnologias acadêmicas, tais como _Haskell_, _C_, dentre outras..., ditam a
evolução da tecnologia e possuem uma comunidade especializada e voltada a
aprendizagem - são as linguagens secundárias, geralmente utilizadas para a
prototipação, prova de conceito e experimentação de ideias.

A base do livro utiliza o dialeto _Lisp_ através dos livros texto:

* _How to Design Programs_ (HtDP); e
  * _Program_
  * _Component_; e
  * _System_
* _Structure and Interpretation of Computer Programs_ (SICP).

=> complemento com os materiais do curso 6.005: _Software Construction_ do
_Massachusetts Institute of Technology_ (MIT).

=> todos os livros estão no capítulo [Referências](referencias.md).

Dentre os dialetos _Lisp_ estão:

* _Racket_;
* _Clojure_ (JVM, CLR e JS);
* _Emacs Lisp_;
* _Common Lisp_;
* _Guile_;
* _Kawa_ (JVM);
* _Fennel_ (_Lua_);
* _Ferret_ (_Embedded Control Systems_)
* ...

## Filosófia

_Em edição..._

* **XDD**: filosofia de desenvolvimento de _software_ formado por:
  Desenvolvimento Guiado por Testes - _Test-Driven Development_ (TDD),
  Desenvolvimento Guiado por Comportamento - _Behavior Driven Development_ (BDD)
  e Projeto Orientado a Domínio - _Domain Driven Design_ (DDD), base para
  modernas arquiteturas baseadas no _Ports-And-Adapters_, tais como:
  _Hexagonal_, _Onion_ e _Clean_.
  * **Desenvolvimento Guiado por Testes** - _Test Driven Development_ (TDD): é
    uma técnica de desenvolvimento de _software_ da Programação Extrema -
    _Extreme Programming_ (XP), em que os testes são criados antes do código de
    produção;
  * **Desenvolvimento Guiado por Comportamento** - _Behavior Driven Development_
    (BDD): é uma técnica de desenvolvimento de _software_ da Programação
    Extrema - _Extreme Programming_ (XP), em que os testes são criados em
    paralelo ao código de produção; e
  * **Projeto Orientado a Domínio** - _Domain Driven Design_ (DDD): aborda um
    compilado de experiências aplicadas ao desenvolvimento de _software_.

## Ciência

_Em edição..._

* **Programação Extrema** - _Extreme Programming_ (XP): metodologia ágil de
  desenvolvimento de _software_ de proposta geral para grupos pequenos e médios;
* **Visão 4+1**: modelagem das visões da arquitetura de _software_ em análise e
  projeto na Linguagem de Modelagem Unificada - _Unified Modeling Language_
  (UML), com aspectos científicos para grupos médios e grandes - definida por
  _Philippe Kruchten_ no artigo _Architectural Blueprints - The "4+1" View Model
  of Software Architecture_ em 1995;
* **Systematic Program Design - SPD**: técnica de desenvolvimento de _software_
  geral para múltiplos paradigmas, recomendado para grupos com expertise; e

## Fluxo

O livro percorre as atividades da construção de _software_ através de:

**[Requisitos](requisitos/README.md)** |
**[Arquitetura](arquitetura/README.md)** |
**[Testes](testes/README.md)** |
**[Código](codigo/README.md)** |
**[Metodologia Científica](metodologia-cientifica/README.md)** | 
**[Referências](referencias.md)**

![](images/arquitetura-software.png)

---

**Atualização de 05/2018**

**Página**: [mdssjc.github.io](http://mdssjc.github.io "Página do MDS") | 
**Repositório**: [github.com/mdssjc](http://github.com/mdssjc "Repositório do MDS")

---
JVM: _Java Virtual Machine_.
CLR: _Common Language Runtime_.
JS: _Java Script_.
