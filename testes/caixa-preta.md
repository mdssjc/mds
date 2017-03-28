# Caixa Preta

A técnica de **teste de caixa preta** (_black-box testing_) tem como objetivo avaliar e verificar o funcionamento externo dos elementos de programação _(técnica funcional)_ durante a etapa de Especificação nas fases de **testes de sistema** ou **testes de aceitação** (_acceptance tests_) quando na presença dos clientes - responsáveis por avaliar o sistema como um todo (**validação**).

* Classes de Equivalência
* Análise de Limites

BDD: _em edição_.

## O Teste

### Documentação

#### Convenções

As seguintes convenções para os identificadores são utilizados:

* Casos de Testes:

  * _NameTest_: testes unitários;
  * _NameIntegrationTest_: testes de integração; e
  * _NameSystemTest_: testes de sistema (ver [Caixa Preta](/testes/caixa-preta.md)).

### Ferramentas

As [ferramentas](ferramentas.md) mais utilizadas são:

* JUnit
* Cucumber
* JBehave
* Web Selenium
* Rest-Assured

## Boas Práticas

* **Test Data Builders**: utilização do padrão de projeto (GoF) _Builder_ para o processo de criação dos objetos para os cenários de testes - auxilia no problema de duplicação de código.

* **Page Object:** abstrair os detalhes de estruturamento da página (DOM) em objetos simples (Navegação e Formulário) no _framework Selenium_.
