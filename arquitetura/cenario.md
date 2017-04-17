# Cenário

O cenário é o processo de transformação (modelagem) dos requisitos em soluções executáveis.

## User Story

O _User Story_ é uma técnica de modelagem da Programação Extrema - _Extreme Programming_ (XP) na qual consiste em uma pequena descrição em linguagem ubíqua das características de valor para o sistema, divididas em cartões de restrição e característica, em que originam as tarefas (_tasks_) e critérios de testes (_test criteria_).

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

**Tarefas**: conjunto de atividades necessárias para criar uma execução da _User Story_.

**Critérios de Testes**: conjuntos de testes para verificar a execução da _User Story_. Em Desenvolvimento Guiado por Comportamento - _Behavior Driven Development_ (BDD) utiliza-se as partes: `Given / When / Then`.

As características de uma boa _User Story_ é resumida no acrônimo _INVEST_:

* _Independent_ - independente;
* _Negotiable_ - negociável;
* _Valuable_ - valorável;
* _Estimatable_ - estimável;
* _Small_ - pequeno; e
* _Testable_ - testável.

A lista de cenários é reunida em uma _Master Story List_, sendo que cada _User Story_ é desenvolvida por completo, ou seja, todas as tarefas são verificadas com testes durante uma iteração.

## Use Case

O _Use Case_ ou Caso de Uso é uma técnica de modelagem clássica para Desenvolvimento Guiado por Caso de Uso - _Use Case Driven Development_ (UCDD) na qual descreve em diferentes níveis através de diagrama (visão geral) e descrição (visão detalhada) as interações dos atores ao sistema.

**Diagrama:**

![](/images/arquitetura-cenario-usecase-1.png)

**Descrição:**

```
Title XYZ
1. Step 1
  1.1 Substep 1.1
2. Step 2
...
```

As partes comportamentais de um _Use Case_ são: título (_title_), atores (_actors_), pré-condições (_preconditions_) e meta (_goal_).

As partes executáveis de um _Use Case_ são: caminho principal (_main path_), caminho alternativo (_alternative path_) e exceções (_exceptions_).

Cada _Use Case_ é desenvolvido por completo e também derivam-se para _Tests Case_ ou Casos de Testes.

## Outros

Existem outras técnicas de modelagem de cénarios, sendo duas comuns _Feature_ e _Especificação de Requisitos_.

### Feature

A _Feature_ é uma técnica de modelagem clássica (Desenvolvimento Guiado por Funcionalidades - _Feature Driven Development_ (FDD)) na qual define uma descrição de alto nível em linguagem ubíqua das funcionalidades/características que o sistema necessita fazer.

```
System XYZ
Features List

1. Feature A;
2. Feature B; and
3. Feature C;
```

Cada _feature_ é desenvolvida por completo, recomenda-se a arquitetura _Package by Feature_.

### Especificação de Requisitos

![](/images/skull.png)

Método obsoleto de modelagem do _Waterfall_.
