# Cenário

O cenário é o processo de transformação \(modelagem\) dos requisitos em soluções executáveis.

## Contexto

_em edição_

## What If

_em edição_

## Use Case

O _Use Case_ ou Caso de Uso é uma técnica de modelagem clássica \(Desenvolvimento Guiado por Caso de Uso - _Use Case Driven Development_ \(UCDD\)\) na qual descreve em diferentes níveis através de diagrama \(visão geral\) e descrição \(visão detalhada\) as interações dos atores ao sistema.

**Diagrama:**

![](/images/arquitetura-cenario-usecase-1.png)

**Descrição:**

```
Título do Cenário
1. Etapa 1
  1.1 Sub-etapa 1.1
2. Etapa 2
...
```

Cada _use case_ é desenvolvido por completo.

## Feature

A _Feature_ é uma técnica de modelagem clássica \(Desenvolvimento Guiado por Funcionalidades - _Feature Driven Development_ \(FDD\)\) na qual define uma descrição de alto nível em linguagem ubíqua das funcionalidades\/características que o sistema necessita fazer.

```
System XYZ
Features List

1. Feature A;
2. Feature B; and
3. Feature C;
```

Cada _feature_ é desenvolvida por completo.

## User Story

O _user story_ é uma técnica de modelagem ágil \(Programação Extrema - _Extreme Programming_ \(XP\)\) na qual consiste em uma pequena descrição em linguagem ubíqua das características de valor para o sistema, divididas em cartões de restrição e característica, em que originam as tarefas \(_tasks_\) e critérios de testes \(_test critteria_\).

**Cartão de Restrição:**

Descrição das restrições e limites do sistema.

```
All resources must load in less than 10 seconds.
```

**Cartão de Característica:**

Descrição das características de uso do sistema.

```
As a < type of user >,   (WHO)  // is this story for
I want < some goal >     (WHAT) // they want to do
so that < some reason >. (WHY)  // they want to do it
```

~~Outro formato aplicado ao BDD é o: ~~~~`Given / When / Then`~~

As características de um bom _User Story_ é resumida no acrônimo _INVEST_:

* _Independent_ - independente;
* _Negotiable_ - negociável;
* _Valuable_ - valorável;
* _Estimatable_ - estimável;
* _Small_ - pequeno; e
* _Testable_ - testável.

A lista de atividades é reunida em uma _Master Story List_.

Cada _user story_ é desenvolvida por completo em uma iteração.

## Especificação de Requisitos

![](/images/skull.png)

Método obsoleto de modelagem.

