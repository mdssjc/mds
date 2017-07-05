# Linguagem de Programação

Processo: _em edição_

Procedimento: _em edição_

Unidade de Significado (Expressões primitivas): os elementos mais simples (atômico) da linguagem.

Meios de Abstração: os elementos compostos podem ser nomeados e manipulados como unidades.

Meios de Combinação: os elementos compostos são construídos a partir de elementos mais simples.

As partes importantes ao aprender uma nova linguagem de programação são:

* **Sintaxe** (_syntax_): as regras de construção da linguagem.
* **Semântica** (_semantics_): significado das características da linguagem, sendo o verificador de tipo (_type-checker_) em tempo de compilação (ambiente estático ou contexto - escopo léxico) para verificação (_type checking_) e/ou inferência (_type inference_) dos tipos; e a avaliação (_evaluation_) das expressões em tempo de execução (ambiente dinâmico ou ambiente - escopo dinâmico) para produção do valor.
* **Expressão Idiomática** (_idioms_): padrões típicos de utilização das características da linguagem.
* **Bibliotecas** (_libraries_): conjunto de código de apoio com o propósito de facilitar o desenvolvimento na linguagem. Aplicação -> _Toolkits_ (Bibliotecas) -> _Frameworks_ (Arcabouços).
* **Ferramentas** (_tools_): programas de auxílio ao desenvolvimento na linguagem, tais como compiladores, interpretadores, depuradores e etc...

## Interpretação

Etapas de interpretação de um programa de computador:

[**Source Code**] --- _code_ ---> [**Tokenizer**] --- _token_ ---> [**Parser**] --- _data structure_ ---> [**Evaluator**]

O código fonte é separado em palavras na qual são analisadas e transformadas em estrutura de dados, assim sendo executadas uma por vez.

## Paradigma

Os paradigmas das linguagens de programação são:

* **Declarativo**
    * Funcional
    * Fluxo de Dados
    * Lógico
* **Imperativo**
    * _Von Neumann_: visão de _software_ sobre a arquitetura do computador, com estruturas de controle (decisão e repetição) e funções.
    * Orientada a Objetos: visão de abstração (antropomorfismo) do mundo real, com encapsulamento, herança e polimorfismo.
    * _Script_: uma forma dinâmica de resolver problemas computacionais.

Muitas linguagens são multiparadigmas, principalmente com um balanço entre Orientada a Objetos/_Script_ e Funcional, alguns casos com DSL em Fluxo de Dados.

## Tipos
