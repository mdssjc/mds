# GRASP

O acrônimo GRASP - _General Responsibility Assignment Software Patterns_ apresentado no livro _Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development_ \(_3rd Edition_\) do autor _Craig Larman_ explana os princípios fundamentais para atribuição de responsabilidades aos elementos de programação da subetapa de Projeto em modelos UML e CRC _Cards_, composto por 9 princípios \(5 básicos - Capítulo 17 e 4 avançados - Capítulo 25\).

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

* **Baixo Acoplamento** - _Low Coupling_: atribuição da responsabilidade de avaliar as dependências entre os elementos de programação.

  Problema: Como auxiliar na redução das dependências, impactos das mudanças e maximização do reuso?

  Solução: Atribua responsabilidades, de modo que o acoplamento \(desnecessário\) mantenha baixo. Use este princípio para avaliar alternativas.

* **Controlador** - _Controller_: atribuição da responsabilidade de manipular os eventos no sistema e delegar aos elementos de programação, também conhecido por Coordenadora_._

  Problema: Qual o primeiro elemento além da camada de apresentação \(visão\) recebe e coordena \(controla\) uma operação no sistema?

  Solução: Atribua a responsabilidade para um elemento representando uma das seguintes escolhas:


> Representa o sistema geral, um elemento raiz, um dispositivo que o _software_ está em execução ou um subsistema maior \(estas são todas variações de um Controlador de Fachada - _Facade Controller or Front Controller_\).
> 
> Representa um cenário de caso de uso em que a operação do sistema ocorre \(um Controlador de Caso de Uso ou de Sessão - _Use Case Controller or Session Controller_\). Identificações comuns são: &lt;name&gt;Handler, &lt;name&gt;Coordinator ou &lt;name&gt;Session.

* **Alta Coesão** - _High Cohesion_: atribuição da responsabilidade de minimizar as funcionalidades não relacionadas aos elementos de programação.

  Problema: Como manter os elementos focados, compreensíveis, gerenciáveis e por consequência, com baixo acoplamento?

  Solução: Atribua responsabilidades de modo que a coesão mantenha alta. Use este princípio para avaliar alternativas.


## Avançados

* **Poliformismo** - _Polymorphism_: atribuição da responsabilidade de manipular variações similares no sistema.

  Problema: Como manipular alternativas baseadas em tipo? Como criar componentes de software plugável?

  Solução: Quando alternativas ou comportamentos relacionados variam por tipo, atribua a responsabilidade para o comportamento usando operações polifórmicas para os tipos pela qual o comportamento varie.

* **Fabricação\/Invenção Pura** - _Pure Fabrication_: atribuição da responsabilidade de decomposição representacional e comportamental do domínio.

  Problema: Qual elemento de programação deveria ter a responsabilidade pela funcionalidade, quando não quer violar os princípios de Alta Coesão e Baixo Acoplamento, ou outras metas, mas a solução oferecida pelo princípio de Especialista na Informação não é apropriado?

  Solução: Atribua o conjunto altamente coesivo de responsabilidades para um elemento de programação artificial ou conveniente que não represente um problema no conceito de domínio, alguma coisa feita para suportar a alta coesão, o baixo acoplamento e o reuso.

* **Indireção** - _Indirection_: atribuição da responsabilidade de mediar componentes do sistema.

  Problema: Onde atribuir uma responsabilidade, para evitar acoplamento direto entre duas \(ou mais\) coisas? Como desacoplar elementos de programação para que o baixo acoplamento é suportado e o potencial reuso mantenha alto?

  Solução: Atribua a responsabilidade para um elemento de programação intermediário para mediar entre outros componentes e serviços de forma que eles não são acoplados diretamente.

* **Variações Protegidas** - _Protected Variations_: atribuição da responsabilidade de proteger os pontos de variação e evolução do sistema_._ Outros nomes: Encapsulamento - _Encapsulation_, Ocultamento de Informação - _Information Hiding_ ou Princípio do Aberto-Fechado - _Open-Closed Principle_.

  Problema: Como projetar elementos de programação, subsistemas e sistemas para que as variações ou instabilidades nesses elementos não tenham impactos indesejáveis sobre outros elementos?

  Solução: Identifique pontos de variação e instabilidade previsível, atribua responsabilidades para criar uma interface estável ao redor.


> Core Protected Variations Mechanisms: recursos da implementados na própria linguagem e sistemas.
> 
> Data-Driven Designs: uso de dados para declaração dos comportamentos do sistema em tempo de execução.
> 
> * Service Lookup: serviço de localização de recursos por nome.
> 
> * Interpreter-Driven Designs: interpretação de código.
> 
> * Reflective or Meta-Level Designs: reflexão e metaprogramação.
> 
> 
> Uniform Access: recurso de propriedade da linguagem.
> 
> Standard Languages: linguagens padronizadas utilizadas internamente.
> 
> The Liskov Substitution Principle: ver [LSP](/arquitetura/solid.md).

