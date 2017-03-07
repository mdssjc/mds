# Projeto

Como fazer para solucionar o problema? No projeto são aplicados os estudos da etapa de **Arquitetura/Análise** em modelos prontos para a implementação na etapa de **Codificação**.

Esses modelos descreve uma visão lógica em relação a cada unidade/tarefa da etapa de **Arquitetura/Cenário** em termos de suas responsabilidades (tipo sabe (atributos) e tipo faz (comportamentos)) e identifica a necessidade de colaboração (relacionamentos).

## CRC Cards

O CRC significa _Class-Responsibility-Collaborator_ \(Classe-Responsabilidade-Colaboração\) e é uma técnica de modelagem ágil \(Programação Extrema - _Extreme Programming_ \(XP\)\).

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

A construção dos CRC _cards_ utiliza a técnica de Análise Textual.

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

Nível 0 -> conjunto concreto

Nível 1 -> estrutura abstrata

A construção do Diagrama de Classe utiliza das técnicas de Análise, principalmente em relação ao domínio.
