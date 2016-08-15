# GRASP

O acrônimo GRASP - _General Responsibility Assignment Software Patterns_ apresentado no livro _Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development_ \(_3rd Edition_\) do autor _Craig Larman_ explana os princípios fundamentais para atribuição de responsabilidades aos elementos de programação da subetapa de Projeto em modelos UML e CRC _Cards_, composto por 9 princípios \(5 básicos e 4 avançados\).

## Básicos

* **Criador** - _Creator_: atribuição da responsabilidade \(fazer\) de criação ao elemento de programação.

  Problema: Quem deve ser responsável por cria uma nova instância de algum elemento?

  Solução: Abribua a B a responsabilidade de criar uma instância de A, se:


> B contém ou agrega A.
> 
> B registra ou guarda instância de A.
> 
> B faz uso de A.
> 
> B tem dados de inicialização de A.

* **Especialista na Informação** - _Information Expert_ \(_Expert_\): atribuição da responsabilidade \(saber e fazer\) ao elemento de programação com a informação.

  Problema: Qual é o princípio fundamental para atribuir responsabilidades aos elementos?

  Solução: Atribua uma responsabilidade para o elemento que tem a informação necessária para cumpri-la.

* **Baixo Acoplamento** - _Low Coupling_: atribuição da responsabilidade de minimizar dependências.

  Problema: Como auxiliar na redução das dependências, impactos das mudanças e maximização do reuso?

  Solução: Atribua responsabilidades, de modo que o acoplamento \(desnecessário\) mantenha baixo. Use este princípio para avaliar alternativas.

* **Controlador** - _Controller_: atribuição da responsabilidade de manipular os eventos no sistema, também conhecido por Coordenadora_._

  Problema: Qual elemento além da camada de apresentação \(visão\) recebe e coordena \(controla\) uma operação no sistema?

  Solução: Atribua a responsabilidade para um elemento representando uma das seguintes escolhas:


> Representa o sistema geral, um elemento raiz, um dispositivo que o _software_ está em execução ou um subsistema maior \(estas são todas variações de um Controlador de Fachada - _Front Controller_\).
> 
> Representa um cenário de caso de uso em que a operação do sistema ocorre \(um Controlador de Caso de Uso ou de Sessão - _Controller_\).

* **Alta Coesão** - _High Cohesion_: atribuição da responsabilidade de minimizar as funcionalidades não relacionadas.

  Problema: Como manter os elementos focados, compreensíveis, gerenciáveis e por consequência, com baixo acoplamento?

  Solução: Atribua responsabilidades de modo que a coesão mantenha alta. Use isto para avaliar alternativas.


## Avançados

* **Poliformismo** - _Polymorphism_: _em edição_;

* **Indireção** - _Indirection_: _em edição_;

* **Fabricação\/Invenção Pura** - _Pure Fabrication_: _em edição_; e

* **Variações Protegidas** - _Protected Variations_: _em edição._


