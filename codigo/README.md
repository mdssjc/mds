# Código

O código é a implementação da solução do problema proposto durante a etapa de Codificação.

**Testes Unitários** - _Unit Testing_: \(ver [Caixa Branca](/testes/caixa_branca.md)\) execução automática de testes para apoiar na etapa de Codificação, em:

* Implementação: das funcionalidade do cenário;
* _FeedBack_: notificação dos problemas no código;
* _Bugs_: previne e corrige os problemas; e
* _Debugging_: reduz a necessidade de uso.

**Refatoração**: técnica de melhoria no código através de correções em padrões de problemas \(~~_code_~~_\_\_\_\_ bad smells\_\):

* [_Refactoring_](http://refactoring.com): catálogo de técnicas sobre refatoração;
* [_SourceMaking_](https://sourcemaking.com): compilado de técnicas para melhoria no código; e
* Dívida Técnica \(_Technical Debt_\): complexidade acumulada durante o desenvolvimento.

**Desenvolvimento Guiado por Testes** - _Test Driven Development_ \(TDD\): técnica na qual empregra os testes como a principal ferramenta de desenvolvimento, antes mesmo do código de produção, através do seu ciclo:

* _Red_ \(_Test Fails_\): exercício do código através de teste - fazer falhar, assim representando cada incremento da especificação;
* _Green_ \(_Test Passes_\): implementação do código - fazer o teste passar; e
* _Refactor_: aplicação da refatoração em melhorias nos recursos utilizados no ciclo, como código, teste, configuração e etc...

**Integração Contínua** - _Continuous Integration_ \(CI\): processo de integração dos incrementos de codificação, com execução automática e avaliativa dos testes - simulando o ambiente de produção. O processo é automático por um sistema de integração contínua, na qual verifica o repositório de código, realiza o _check-in\/build_ e analisa a saúde do projeto, notificando os problemas aos desenvolvedores.

