# Código

![](../images/codigo.png)

A etapa de **Codificação** traz a implementação da solução do problema proposto em código (produto do projeto).

```
+-------+      +---+      +-------------+
|CLIENTE| <--> |API| <--> |IMPLEMENTAÇÃO|
+-------+      +---+      +-------------+
```

**Desenvolvimento Guiado por Testes** - _Test Driven Development_ (TDD): é uma técnica de desenvolvimento de _software_ da Programação Extrema - _Extreme Programming_ (XP), em que os testes são criados antes do código de produção, através do seu ciclo:

* _Red_ (_Test Fails_): criação da Interface de Programação de Aplicativos - _Application Programming Interface_ (API) com o exercício de uma parte do comportamento da tarefa (_User Story_) através do código de [Testes](../testes/README.md) - fazer falhar, assim representando cada incremento do cenário;
* _Green_ (_Test Passes_): implementação do código - fazer o teste passar; e
* _Refactor_: aplicação da refatoração em melhorias nos recursos utilizados no ciclo, como código, teste, configuração e etc...

Escrever os testes antes do código melhora a estrutura do projeto, pois traz _feedback_ mais cedo e apredizado constante.

**Refatoração** - _Refactoring_: é uma técnica de melhoria na estrutura interna do código, sem alterar seu comportamento, através de correções em padrões de problemas (_bad smells_):

* _[Refactoring](http://refactoring.com)_: catálogo de técnicas sobre refatoração;
* _[SourceMaking](https://sourcemaking.com)_: compilado de técnicas para melhoria no código;
* Dívida Técnica (_Technical Debt_): complexidade acumulada durante o desenvolvimento;
* Código Legado: código antigo e com características fora do padrão de desenvolvimento; e
* [_Design smells_](../arquitetura/solid.md): sintomas de um projeto ruim.

**Integração Contínua** - _Continuous Integration_ (CI): é um processo da Programação Extrema - _Extreme Programming_ (XP) para a integração dos incrementos de codificação, com execução automática e avaliativa dos testes - simulando o ambiente de produção. O processo é automático por um sistema de integração contínua, na qual verifica o repositório de código, realiza o _check-in/build_ e analisa a saúde do projeto, notificando os problemas aos desenvolvedores.

**Programação por Contrato**: o cliente aceita as regras (obrigações e benefícios) de como manipular os problemas pelo uso incorreto da Interface de Programação de Aplicação - _Application Programming Interface_ (API) - geralmente verificando as pré-condições, pós-condições e invariâncias; e retornando um valor nulo, opcional ou lançando uma exceção - uma representação de falha.
    * Pré-condição: indica uma violação pelo cliente, falhou em não observar as condições impostas na sua chamada.
    * Pós-condição: indica uma violação pela implementação, falhou em entregar sua promessa.
    * Invariância: indica uma propriedade na qual deve ser satisfeita pelo cliente e preservada pela implementação.

**Programação Defensiva**: a Interface de Programação de Aplicação - _Application Programming Interface_ (API) protege o cliente do uso incorreto - geralmente realizando checagens nos valores de entrada e retornando um resultado padrão ou lançando uma exceção com tratamento obrigatório.
