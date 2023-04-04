# LIVRO DO MDS

A ideia por trás desse projeto foi inspirada pelos livros _Pragmatic Thinking and Learning - Refactor Your "Wetware"_ do autor _Andy Hunt_ e _The Pragmatic Programmer: From Journeyman to Master_ dos autores _Andrew Hunt_ e _David Thomas_. Ambos os livros abordam a importância de se criar um "cérebro externo" para registro e organização dos estudos e aprendizados.

O projeto tem a composição de:

![Composição do Projeto](./assets/introduction-project-composition.png 'Composição do Projeto')

- [o livro](https://github.com/mdssjc/mds/ 'o livro') (atemporal): livro na qual explora diversos tópicos relacionados ao desenvolvimento de software, com foco em boas práticas e técnicas modernas;
- [a página](https://marcelo-mds.dev/ 'a página') (temporal): página pessoal com informações sobre experiências e projetos relacionados ao desenvolvimento de software;
- [as notas](https://github.com/mdssjc/mds-notes/ 'as notas') (fragmentos): repositório de anotações sobre diversos tópicos relacionados ao desenvolvimento de software e assuntos relacionados; e
- [o repositório](https://github.com/mdssjc/ 'o repositório') (construção): repositório principal do projeto com o código-fonte e as contribuições na forma de experiências e estudos.

## Para Quem é Este Livro?

Este livro destina-se a todos que desejam aprimorar suas habilidades na profissão de **_Craftsman_ - Construtor de _Software_**. Se você é um iniciante na programação, recomendamos que estude a lógica de programação antes de continuar com o livro, em breve será adicionado apêndices sobre como ingressar na profissão. Na página, você encontrará dojos e/ou atividades específicas para iniciantes em programação.

## Objetivos

- Compilar os conhecimentos/sabedorias utilizados pelo _Craftman_.
- Explanar um modelo de desenvolvimento base com fácil aplicação em modelos utilizados no mercado.
- Sugerir os pontos de estudos para a evolução dos temas.

## Introdução

O livro é um guia para você leitor carregar durante sua carreira de _Craftman_ com temas pragmaticamente voltados para a construção de _softwares_ na categoria de aplicações.

Os capítulos descrevem as etapas marco de um fluxo de desenvolvimento de _software_ geral, considerando uma base sólida como também os aspectos filosóficos e científicos do processo, assim como seus pontos de extensão.

### Fluxo de Desenvolvimento

O fluxo de desenvolvimento utilizado pelo _Craftman_ tem a seguinte composição:

![Fluxo de Desenvolvimento](./assets/introduction-development-flow.png 'Fluxo de Desenvolvimento')

### A Linguagem

As linguagens de programação são geralmente classificadas em três categorias: _mainstream_, modernas e acadêmicas.

- **Mainstream**: são as linguagens mais amplamente utilizadas na indústria de _software_ devido à sua confiabilidade, grande variedade de plataformas e bibliotecas disponíveis, bem como à sua adaptação às máquinas atuais. Essas linguagens são usadas para resolver problemas em geral e possuem uma grande comunidade de entusiastas e evangelistas. Alguns exemplos de linguagens _mainstream_ incluem _Java_, _C#,_ _C++_, _JavaScript_, _Python_ e _Ruby_.

- **Modernas**: são as linguagens de programação criadas recentemente para atender às necessidades específicas do mercado. Elas trazem novas ideias e abordagens para resolver problemas, visando aumentar a produtividade e a segurança. Exemplos de linguagens modernas incluem _Dart_, _Rust_, _Kotlin_, _Swift_, _Go_, _V_ e _Zig_.

- **Acadêmicas**: são as linguagens de programação que são usadas principalmente no ambiente acadêmico para pesquisa e experimentação de ideias. Essas linguagens são frequentemente usadas para ensinar conceitos avançados de programação e ciência da computação. Alguns exemplos de linguagens acadêmicas incluem _Haskell_, _Racket_, _Lisp_, _ML_ e _Prolog_.

As linguagens de programação escolhidas para este livro são o _Dart_, que será utilizada em conjunto com a plataforma _Flutter_ e seu ecossistema para tarefas gerais, e a linguagem _Rust_, juntamente com seu ecossistema, para estruturas mais complexas. A escolha dessas duas linguagens visa fomentar a adoção de uma mentalidade (_mindset_) de usar uma linguagem secundária para atividades complementares.

### A Filosofia

A filosofia do _Craftman_ é composta por três importantes técnicas de desenvolvimento de _software_: TDD, BDD e DDD.

- **Desenvolvimento Guiado por Testes (TDD)**: é uma técnica da Programação Extrema (XP) que consiste em escrever os testes antes do código de produção, em um ciclo de falha-passa-refatora. Essa abordagem visa garantir a qualidade do código e reduzir a quantidade de _bugs_.

- **Desenvolvimento Guiado por Comportamento (BDD)**: é uma técnica derivada do TDD que utiliza a linguagem do domínio e foca no comportamento esperado do sistema. Em conjunto com práticas de _Domain Driven Design_ (DDD) e _Object-Oriented Analysis and Design_ (OOAD), os testes são criados em paralelo ao código de produção, permitindo uma melhor comunicação entre as equipes de desenvolvimento e negócios.

- **Projeto Orientado a Domínio (DDD)**: é uma abordagem que reúne um conjunto de experiências e práticas para o desenvolvimento de _software_. O DDD se concentra em modelar o domínio do problema, utilizando conceitos como entidades, valores, serviços e agregados para criar um código mais expressivo e sustentável ao longo do tempo.

### A Ciência

A ciência do _Craftman_ é composta por três elementos essenciais para os desenvolvedores de _software_: _Circle of Life and Pomodoro_, _Clean Design_ e Pergaminhos.

- **Circle of Life and Pomodoro**: são duas ferramentas poderosas para maximizar a produtividade e alcançar objetivos de maneira eficiente e saudável. A combinação dessas ferramentas pode ajudar a gerenciar melhor o tempo e o trabalho, levando a melhores resultados e satisfação pessoal e profissional.

- **Clean Design**: é uma metodologia criada pelo autor _Robert C. Martin_, também conhecido como _Uncle Bob_, que prioriza a clareza, simplicidade e facilidade de manutenção do código em todas as fases do processo de desenvolvimento de _software_. Esses princípios ajudam a criar sistemas mais eficientes e sustentáveis.

- **Pergaminhos**: são um conjunto de conhecimentos e experiências que têm sido utilizados e aprimorados por desenvolvedores de _software_ ao longo dos anos na forma de práticas, princípios e padrões.

## Capítulos

- [Capa](cover.md 'Capa')
- [Introdução](readme.md 'Introdução')
- [Pergaminhos](scrolls/readme.md 'Pergaminhos')
- [Requisitos](requirements/readme.md 'Requisitos')
- Arquitetura
- [Testes](testing/readme.md 'Testes')
- [Código](coding/readme.md 'Código')
- Monitoramento
- Metodologia
- Conclusão
- [Referências](references.md 'Referências')

## Observação

Para visualizar a versão antiga do livro, acesse a `branch old`.

O foco será em utilizar o _Dart_ e o _Rust_, porém como toda ferramenta, poderá ser alterada/adicionada com a necessidade, conforme a proposta do livro em utilizar um ecossistema para resolução de problemas.

O livro ainda está em desenvolvimento e, como qualquer projeto em andamento, pode conter erros ou imprecisões. Estes serão corrigidas na próxima versão de Abril.

## Data da Atualização

30/04/2023
