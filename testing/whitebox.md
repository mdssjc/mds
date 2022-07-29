# CAIXA BRANCA

A técnica de **teste de caixa branca** (_white-box testing_) tem como objetivo avaliar a estrutura interna dos elementos de programação _(técnica estrutural)_ durante a etapa de Codificação nas fases de **testes unitários** (_unit testing_) - responsáveis por auxiliar e avaliar no desenvolvimento dos cenários de uma unidade de código (estrutura interna do programa) e/ou **testes de integração ou componentes** (_integration testing or component testing_) - responsáveis por avaliar a comunicação entre unidades e recursos, principalmente a camada de infraestrutura e códigos de terceiros (**verificação**).

Durante o desenvolvimento de _software_, os testes auxiliam nas técnicas de:

- **Desenvolvimento Guiado por Testes** - _Test Driven Development_ (TDD);
- **Refatoração** - _Refactoring_;
- **Cobertura de Testes** - _Test Coverage_;
- **Integração Contínua** - _Continuous Integration_ (CI); e
- **Testes de Regressão** - _Regression Testing_.

Outras características apresentadas são:

- Implementação: das funcionalidades do cenário;
- _FeedBack_: notificação dos problemas no código;
- _Bugs_: previne e corrige os problemas; e
- _Debugging_: reduz a necessidade de uso.

O teste é divido em unidades de testes, em que é o menor elemento de programação de uma dada tecnologia, tais como: funções, comandos, macros, métodos, classes, dentre outros...

Os excessos na unidade de teste (padrões de _feedback_) diz o quanto estável é a unidade de programação:

- exercícios das responsabilidades: baixa coesão;
- dublês das colaboradoras: alto acoplamento; e
- avaliação em colaboradoras: encapsulamento.

Complexidade ciclomática: métrica das ramificações existentes em uma unidade de programação, quanto maior o número, mais complexo e difícil de ser testado será o _software_ (mais informações em [Medindo a complexidade do seu código](http://blog.caelum.com.br/medindo-a-complexidade-do-seu-codigo/ 'Medindo a complexidade do seu código')).

## O Teste

O teste utiliza as tarefas do cenário para a composição de um conjunto de casos de teste durante a etapa de Codificação, assim descrevendo **o que** cada estrutura de programação deve fazer para garantir a **verificação** da Arquitetura.

Na elaboração dos casos de teste utiliza uma identificação e um nome descritivo para cada variação de uma específica funcionalidade do cenário - formando uma execução atômica, assim definindo seus dados de testes como entrada e sua saída esperada na execução, conforme o estado inicial.

`{ ID; Nome do Teste; Entrada; Saída Esperada; Estado Inicial }`

**Exemplo:**

```
| ID  | Nome do Teste   | Entrada    | Saída Esperada | Estado Inicial            |
|-----+-----------------+------------+----------------+---------------------------|
|  1  | Testando o A... | "variável" | "variável"     | Objeto Contador existente |
|     |                 | 20         | 123            |                           |
|-----+-----------------+------------+----------------+---------------------------|
|  2  | Testando o B... | N/A        | "variável"     | Objeto Contador com valor |
|     |                 |            | 345            | padrão de 345             |
|-----+-----------------+------------+----------------+---------------------------|
| ... |                 |            |                |                           |
```

Os casos de teste são organizadas em quatro (4) fases/etapas, sendo:

- **setup** ou **arrange**: construção e configuração dos estados (entradas, condições e limites) requeridos pelo caso de teste;
- **exercise** ou **act**: execução das funcionalidades do código sobre teste;
- **verify** ou **assert**: avaliação dos estados e comportamentos do código, comparando os resultados obtidos com as saídas esperadas; e/ou
- **teardown** ou **after**: liberação dos recursos utilizados pelo código.

**Importante o cuidado** para não violar o Princípio da Responsabilidade Única - _Single Responsibility Principle_ (SRP) durante a implementação do código sobre teste, pois deve-se testar apenas as funcionalidades expostas (_Tell, Don't Ask_) sem o encadeamento de mensagens (_Law of Demeter_), a proposta básica é que cada **Classe de Equivalência** deva possuir um caso de teste único e suficiente, ou seja, a inclusão de pequenos incrementos entre testes conforme suas condições limites.

## Documentação

Os testes formam a documentação viva do código, em que são de extrema importância seus identificadores (nomes dos testes) serem pensadas ao nível sintático (relação entre os termos) e semântico (sentido de ideias) com o que será testado.

### Convenções

As seguintes convenções para os identificadores são utilizados:

- Casos de Testes:

  - _NameTest_: testes unitários;
  - _NameIntegrationTest_: testes de integração; e
  - _NameSystemTest_: testes de sistema (ver Caixa Preta).

- Testes:

  - _Action_: utiliza uma ação avaliável do teste, considerando o resultado e/ou condição da operação, exemplo: _adicionaUmUsuarioEmUmaListaVazia_;
  - _Given-When-Then_: relaciona o contexto, ação e resultado do teste, exemplo: _dadoXQuandoAcontecerYEntaoFacaZ_; e
  - _Helper Objects_: nomeia os comandos em modo imperativo e as avaliações em modo indicativo, exemplo: _dispareUmSinalDeFalha_ e _mostraAOcorrenciaDaFalha_.

### Dicas

Os identificadores tendem a ficarem longo, assim dificultando em sua leitura - uma dica é utilizar _underscore_ sobre o _camel case_, conhecido também por _snake case_:

`requisitarUmaMensagemComRepositorioVazio` para `requisitar_uma_mensagem_com_repositorio_vazio`
