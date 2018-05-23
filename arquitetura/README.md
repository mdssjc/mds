# Arquitetura

![](../images/arquitetura.png)

A etapa de **Arquitetura** traz a estrutura organizacional de um sistema,
incluindo sua decomposição em partes, sua conectividade, seus mecanismos de
interação e os princípios e decisões que orientam no desenvolvimento de um
sistema.

```
[Gather Requirements] -> [Analyze in Real World Context] -> [Develop the Architecture]
```

As três fundamentais etapas são:

* [**Cenário**](cenario.md "Cenário"): Descrevendo o problema.
* [**Análise**](analise.md "Análise"): O que fazer para solucionar o problema?
* [**Projeto**](projeto.md "Projeto"): Como fazer para solucionar o problema?

O guia para etapas são através dos **Princípios, Padrões e Práticas**.

## Princípios, Padrões e Práticas

Os princípios, padrões e práticas são as bagagens de experiências do
desenvolvedor sobre a etapa de [**Arquitetura**](README.md "Arquitetura") - com
a adição de _complexidade adicional_ na maioria dos casos: enquanto os
princípios trazem as sugestões e recomendações de expressões idiomáticas para a
criação do _software_, os padrões trazem a formalização dos princípios em pares
de problema/solução para serem aplicados e moldados aos contextos de _software_,
por fim as práticas trazem as atividades/técnicas executadas durante o projeto
pela abordagem **filosófica** e **científica**.

Os problemas são:

```
detectados pelas Práticas,
diagnosticados pelos Princípios,
solucionados pelos Padrões, e
regulados pelos Antipadrões.
```

Os mais utilizados/aplicados são:

* [Práticas](praticas.md "Práticas") (Práticas Comuns)
* [Princípios](principios.md "Princípios") (Princípios Gerais)
* [SOLID](solid.md "SOLID") (Princípios de Projeto)
* [GRASP](grasp.md "GRASP") (Padrões Fundamentais)
* [PLoP](plop.md "PLoP") (Padrões de Projeto)
* [GoF](gof.md "GoF") (Padrões de Projeto)
* [POSA](posa.md "POSA") (Padrões de Arquitetura)
* [Antipadrões](antipadroes.md "Antipadrões") (Antipadrões)

Pontos importantes:

* **Trade-off**: os padrões de projeto são utilizados conforme um equilíbrio entre
  espaço e tempo dos recursos computacionais.

## Outros

Dentre os pontos importantes estão:

* **Etapa Zero**: a etapa/iteração zero é a primeira atividade, na qual utiliza
  o cenário mais simples (_World_ ou _Walking Skeleton_) e representativo do
  projeto, assim validando o ambiente de desenvolvimento (IDE, Controle de
  Versão, Servidores, _Frameworks_, _Rigs_, etc...).
* **Arquiteturas Modernas**: novos estudos de arquiteturas para a representação
  de _software_, baseadas em variantes da arquitetura _Ports-And-Adapters_, tais
  como: _Hexagonal_, _Onion_ e _Clean_.
