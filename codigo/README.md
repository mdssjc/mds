# Código

![](/images/codigo.png)

O código é a implementação da solução do problema proposto durante a etapa de Codificação.

```
+-------+      +---+      +-------------+
|CLIENTE| <--> |API| <--> |IMPLEMENTAÇÃO|
+-------+      +---+      +-------------+
```

**Testes Unitários** - _Unit Testing_: \(ver [Caixa Branca](/testes/caixa-branca.md)\) execução automática de testes para apoiar na etapa de Codificação, em:

* Implementação: das funcionalidade do cenário;
* _FeedBack_: notificação dos problemas no código;
* _Bugs_: previne e corrige os problemas; e
* _Debugging_: reduz a necessidade de uso.

**Refatoração** (_Refactoring_): técnica de melhoria no código através de correções em padrões de problemas \(_bad smells_\):

* _[Refactoring](http://refactoring.com)_: catálogo de técnicas sobre refatoração;
* _[SourceMaking](https://sourcemaking.com)_: compilado de técnicas para melhoria no código;
* Dívida Técnica \(_Technical Debt_\): complexidade acumulada durante o desenvolvimento; e
* Problemas comuns: Rigidez (_Rigidity_), Fragilidade (_Fragility_), Imobilidade (_Immobility_), Viscosidade (_Viscosity_), Complexidade Desnecessária (_Needless Complexity_), Repetição Desnecessária (_Needless Repetition_) e Opacidade (_Opacity_).

Livro de referência: _Refactoring: Improving the Design of Existing Code_.

**Desenvolvimento Guiado por Testes** - _Test Driven Development_ \(TDD\): técnica na qual emprega os testes como a principal ferramenta de desenvolvimento, antes mesmo do código de produção, através do seu ciclo:

* _Red_ \(_Test Fails_\): exercício do código através de teste - fazer falhar, assim representando cada incremento da especificação;
* _Green_ \(_Test Passes_\): implementação do código - fazer o teste passar; e
* _Refactor_: aplicação da refatoração em melhorias nos recursos utilizados no ciclo, como código, teste, configuração e etc...

**Integração Contínua** - _Continuous Integration_ \(CI\): processo de integração dos incrementos de codificação, com execução automática e avaliativa dos testes - simulando o ambiente de produção. O processo é automático por um sistema de integração contínua, na qual verifica o repositório de código, realiza o _check-in/build_ e analisa a saúde do projeto, notificando os problemas aos desenvolvedores.

---

**Programação por Contrato**: o cliente aceita as regras de como manipular os problemas pelo uso incorreto da API - geralmente retornando um valor nulo ou lançando uma exceção.

**Programação Defensiva**: a API protege o cliente do uso incorreto - geralmente retornando um resultado padrão ou lançando uma exceção com tratamento obrigatório.

