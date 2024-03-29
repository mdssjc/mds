# CAIXA PRETA

A técnica de **teste de caixa preta** (_black-box testing_) tem como objetivo avaliar e verificar o funcionamento externo dos elementos de programação _(técnica funcional)_ durante a etapa de Especificação nas fases de **testes de sistema** e/ou **testes de aceitação** (_acceptance tests_) quando na presença dos clientes - responsáveis por avaliar o sistema como um todo (**validação**).

Durante o desenvolvimento de _software_, os testes auxiliam nas técnicas de:

- **Projeto de Programa Sistemático** - _Systematic Program Design_ (SPD); e
- **Desenvolvimento Guiado por Comportamento** - _Behavior Driven Development_ (BDD).

## O Teste

Os testes tem como objetivos:

- Funcionalidade;
- Validação de dados;
- Saída de resultados;
- Transição de estados; e
- Equivalências e Limites.

Com auxílio dos desenvolvedores: verificação de auditoria e _logging_, dados para outros sistemas, informações do sistema e recursos utilizados.

## Documentação

Os testes formam a documentação viva do código, em que são de extrema importância seus identificadores (nomes dos testes) serem pensadas ao nível sintático (relação entre os termos) e semântico (sentido de ideias) com o que será testado.

### Convenções

As seguintes convenções para os identificadores são utilizados:

- Casos de Testes:

  - _NameTest_: testes unitários (ver [Caixa Branca](whitebox.md.md 'Caixa Branca'));
  - _NameIntegrationTest_: testes de integração (ver [Caixa Branca](whitebox.md 'Caixa Branca')); e
  - _NameSystemTest_: testes de sistema.

## Boas Práticas

- **Test Data Builders**: utilização do padrão de projeto (GoF) _Builder_ para o processo de criação dos objetos para os cenários de testes - auxilia no problema de duplicação de código.

- **Page Object:** abstração/encapsulamento dos detalhes de estruturamento da interface gráfica em objetos simples (Navegação e Formulário) para _frameworks_ de Interface do Usuário - _User Interface_ (UI).
