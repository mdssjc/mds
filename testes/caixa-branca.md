# Caixa Branca
Os testes de caixa branca (*white-box testing*) são conhecidos como **testes unitários** *[técnica estrutural]*, responsáveis por auxiliar e avaliar no desenvolvimento dos cenários de uma unidade de código (estrutura interna do programa). **Importante o cuidado** para não violar o Princípio da Responsabilidade Única - *Single Responsibility Principle* (SRP) durante a implementação do código sobre teste, pois deve-se testar apenas as funcionalidades expostas (*Tell, Don't Ask*). Esses testes são tratados como a documentação do código, assim deve-se sua identificação serem pensadas em nível sintático e semântico, as próprias ferramentas de testes incentivam essa técnica como por exemplo o JUnit e Hamcrest.

Esta é uma ferramenta essencial no Desenvolvimento Guiado por Testes - *Test Driven Development* (TDD). Em ferramentas de Integração Contínua - *Continuous Integration* (CI) ocorre a execução automática e avaliativa dos testes.

A proposta básica é que cada **Classe de Equivalência** deve possuir um cenário de teste único.

**Ferramentas:**

* assert (avaliação de sanidade em código)
* JUnit (base dos testes)
* Hamcrest (expressividade na avaliação do código)
* Mockito (dublê de objetos)
* Infinitest (automação da execução dos testes no cliente)

**Documentação:**

Os testes formam a documentação do código, logo seus nomes são de extrama importância, como:

* **action**: usa uma ação do cenário de teste, ex: *adicionaUmUsuario*.

* **given-when-then**: relaciona o contexto, ação e resultado, ex: *dadoXQuandoAcontecerYEntaoFacaZ*.

**Técnicas:**

* **AAA[A]** - organização e formatação dos testes:

  **A**rrange: monta/organiza o cenário do código com todas as entradas e pré-condições necessárias;

  **A**ct: exercita/executa o código sobre teste;

  **A**ssert: avalia os resultados do código com os esperados;

  **A**fter: finaliza os recursos utilizados no teste.

* **FIRST** - propriedades de bons testes:

  **F**ast: rápidos em sua execução, assim mais testes serão avaliados;

  **I**solated: isolados dos outros códigos, assim a verificação da falha será óbvia;

  **R**epeatable: possui repetibilidade em qualquer ordem e tempo;

  **S**elf-validating: automação em sua execução e avaliação;

  **T**imely: em momento oportuno, escreva os testes antes do código.

* **B->RIGHT**

*em edição*
 
* **CORRECT**

*em edição*

**Usos:**

* **TDD**: utiliza os testes como principal ferramenta de desenvolvimento através do seu ciclo:
  
  **Red**: o teste representa cada requisito.

  **Green**: o teste guia a implementação do código.

  **Refactor**: os testes mantém a integridade do código.
  
* **CI**: *em edição*

**Boas Práticas:**

* **Identificação:** utilização do nome da classe seguido por Test.

* **Test Data Builders:** utilização do padrão de projeto Builder para construção dos objetos para cenário de testes.

* **Adapters:** utilização para testes com métodos estáticos.

* **Mock Objects:** isolação de funcionalidades com dependência externa.

* **Baby Steps:** incrementos em pequenos passos, assim ganhando confiança.