# Caixa Branca
Os testes de caixa branca são conhecidos como testes unitários, responsáveis por avaliar e auxiliar no desenvolvimento dos cenários de uma unidade de código.

**Ferramentas:**
* JUnit (base dos testes)
* Hamcrest (expressividade de código)
* Mockito (dublê de objetos)
* Infinitest (automação)

Cada **Classe de Equivalência** deve possuir um cenário de teste único.

### AAA[A]
**A**rrange: montar/organizar o cenário do código;

**A**ct: exercitar/executar o código;

**A**ssert: avaliar os resultados do código;

**A**fter: finalizar recursos utilizados no teste.

### FIRST
### B->RIGHT
### CORRECT

**Boas Práticas:**

**Identificação:** utilização do nome da classe seguido por Test.

**Test Data Builders:** utilização do padrão de projeto Builder para construção dos objetos para cenário de testes.

**Adapters:** utilização para testes com métodos estáticos.

**Mock Objects:** isolação de funcionalidades com dependência externa.