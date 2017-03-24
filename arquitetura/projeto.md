# Projeto

Como fazer para solucionar o problema? No projeto são aplicados os estudos da subetapa de [**Análise**](/arquitetura/analise.md) em modelos prontos para a implementação na etapa de [**Codificação**](/codigo/README.md).

Esses modelos descreve uma visão lógica em relação a cada unidade/tarefa da subetapa de [**Cenário**](/arquitetura/cenario.md) em termos de papéis com específicas responsabilidades (tipo sabe (atributos) e tipo faz (comportamentos)) e interação pela necessidade de colaboração (relacionamentos).

## Cartão CRC

O cartão Classe-Responsabilidade-Colaboração - _Class-Responsibility-Collaborator_ (CRC) é uma técnica de modelagem da Programação Extrema - _Extreme Programming_ (XP) na qual utiliza a técnica de Análise Textual nos cenários para formar os elementos de programação.

**Exemplo de Cartão:**

```
Class: NameOfClass
-------------------------------------------
Description: description of responsibility.
-------------------------------------------
Responsibilities:
Name  |  Collaborator
------+--------------
Do    |  OtherClass
Know  |  -
```

**Etapas:**

* Obtenção do Cenário;
* Identificação dos Substantivos como Classes;
* Refinamento da Lista de Classes;
* Identificação das Responsabilidades Óbvias;
* Identificação dos Verbos como Responsabilidades;
* Atribuição das Novas Responsabilidades;
* Apresentação da Lógica para cada Responsabilidade.

## Diagrama de Classe

O Diagrama de Classe é uma técnica de modelagem em Linguagem de Modelagem Unificada - _Unified Modeling Language_ (UML).

![](/images/arquitetura-projeto-diagrama-classe.png)

Em PlantUML:

```
@startuml

title Class Diagram

class ClassA {
  +Type attribute
  +Type operation()
}

class ClassB {
  +Type attribute
  +Type operation()
}

ClassA --> ClassB

@enduml
```

Nível 0 -> conjunto concreto das instâncias de dados

Nível 1 -> estrutura abstrata do modelo de dados

A construção do Diagrama de Classe utiliza das técnicas de Análise, principalmente em relação ao domínio.
