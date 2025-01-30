# INTRODUÇÃO

A ideia por trás desse projeto foi inspirada pelos livros _Pragmatic Thinking and Learning - Refactor Your "Wetware"_ do autor _Andy Hunt_ e _The Pragmatic Programmer: From Journeyman to Master_ dos autores _Andrew Hunt_ e _David Thomas_. Ambos os livros abordam a importância de se criar um "cérebro externo" para registro e organização dos estudos e aprendizados.

O projeto tem a composição de:

![Composição do Projeto](./assets/introduction-project-composition.png 'Composição do Projeto')

- [o livro](https://github.com/mdssjc/mds/ 'o livro') (atemporal): livro na qual explora diversos tópicos relacionados ao desenvolvimento de _software_, com foco em boas práticas e técnicas modernas;
- [a página](https://marcelo-mds.dev/ 'a página') (temporal): página pessoal com informações sobre experiências e projetos relacionados ao desenvolvimento de _software_;
- [as notas](https://github.com/mdssjc/mds-notes/ 'as notas') (fragmentos): repositório de anotações sobre diversos tópicos relacionados ao desenvolvimento de _software_ e assuntos relacionados; e
- [o repositório](https://github.com/mdssjc/ 'o repositório') (construção): repositório principal do projeto com o código-fonte e as contribuições na forma de experiências e estudos.

## Para Quem é Este Livro?

Este livro destina-se a todos que desejam aprimorar suas habilidades na profissão de **_Craftsman_ - Construtor de _Software_**, explorando a cultura da criação de soluções e resolução de problemas por meio da programação. Se você está iniciando sua jornada no desenvolvimento de _software_, recomendamos começar estudando lógica de programação antes de prosseguir com o conteúdo deste livro. Em breve, serão adicionados apêndices com orientações detalhadas sobre como ingressar na área. Além disso, na página do projeto, você encontrará dojos e atividades práticas especialmente desenvolvidas para iniciantes.

## Objetivos

- Compilar os conhecimentos e práticas fundamentais utilizados por um _Craftsman_ no desenvolvimento de _software_.
- Apresentar um modelo de desenvolvimento base, de fácil aplicação e alinhado às práticas comuns no mercado.
- Sugerir tópicos de estudo que promovam a evolução contínua nos temas abordados.

## O que é este livro?

Este livro é um guia prático para desenvolvedores de _software_, com foco em construir aplicações de qualidade. Os capítulos abordam desde os fundamentos da programação até práticas essenciais para garantir a entrega de um produto de qualidade.

Ao longo do livro, exploramos as etapas fundamentais do desenvolvimento de _software_, incluindo o entendimento dos requisitos, a definição da arquitetura, os testes, o desenvolvimento de código e o monitoramento. Além disso, discutimos aspectos filosóficos e científicos do processo, bem como seus pontos de extensão.

Se você é um iniciante na área de programação ou um desenvolvedor experiente que busca aprimorar suas habilidades, este livro é para você. Aproveite a leitura e aplique o conhecimento adquirido em seus projetos para se tornar um **_Craftman_** de sucesso!

### A Linguagem

As linguagens de programação são geralmente classificadas em três categorias: _mainstream_, modernas e acadêmicas.

- **Mainstream**: são as linguagens mais amplamente utilizadas na indústria de _software_ devido à sua confiabilidade, grande variedade de plataformas e bibliotecas disponíveis, bem como à sua adaptação às máquinas atuais. Essas linguagens são usadas para resolver problemas em geral e possuem uma grande comunidade de entusiastas e evangelistas. Alguns exemplos de linguagens _mainstream_ incluem _Java_, _C#,_ _C++_, _JavaScript_, _Python_ e _Ruby_.

- **Modernas**: são as linguagens de programação criadas recentemente para atender às necessidades específicas do mercado. Elas trazem novas ideias e abordagens para resolver problemas, visando aumentar a produtividade e a segurança. Exemplos de linguagens modernas incluem _Dart_, _Rust_, _Kotlin_, _Swift_, _Go_, _V_ e _Zig_.

- **Acadêmicas**: são as linguagens de programação usadas principalmente no ambiente acadêmico para pesquisa e experimentação de ideias. Essas linguagens são frequentemente usadas para ensinar conceitos avançados de programação em ciência da computação. Alguns exemplos de linguagens acadêmicas incluem _Haskell_, _Racket_, _Lisp_, _ML_ e _Prolog_.

O livro utiliza a linguagem de programação _Dart_ para apresentar os conceitos, enquanto outras linguagens são exploradas como complemento para o conteúdo do livro através das seções do **Caminho do Código** (que oferece implementações em diferentes linguagens), **Laboratório do Código** (com _links_ para experimentos, dojos e outros materiais) e o **Ei, olha isso!** (que traz destaques e comparações com outras linguagens).

### A Filosofia

A filosofia do _Craftman_ é composta por três importantes técnicas de desenvolvimento de _software_: Desenvolvimento Orientado pela Qualidade, Lentes e Lógica.

- **Desenvolvimento Orientado pela Qualidade**: TDD, BDD e DDD são técnicas de desenvolvimento de _software_ que se concentram em diferentes aspectos da construção de um sistema de qualidade. O TDD (Desenvolvimento Guiado por Testes) enfatiza a criação de testes automatizados para garantir a qualidade do código e reduzir a quantidade de _bugs_. O BDD (Desenvolvimento Guiado por Comportamento) utiliza a linguagem do domínio para focar no comportamento esperado do sistema, permitindo uma melhor comunicação entre as equipes de desenvolvimento e negócios. O DDD (Projeto Orientado a Domínio) se concentra em modelar o domínio do problema para criar um código mais expressivo e sustentável ao longo do tempo. Utilizando essas técnicas em conjunto, é possível desenvolver _software_ de alta qualidade, que atenda às necessidades dos usuários e dos negócios de forma eficiente.

- **Lentes**: paradigmas são modelos de pensamento que definem como os problemas devem ser abordados e resolvidos na programação. O paradigma da Programação Orientada a Objetos (POO) é baseado na ideia de que tudo é um objeto, que possui atributos e comportamentos. Já o paradigma da Programação Funcional (PF) se concentra na manipulação de funções como objetos de primeira classe, evitando efeitos colaterais e promovendo a imutabilidade dos dados. Cada paradigma tem seus próprios prós e contras e, escolher o mais adequado para cada situação é fundamental para desenvolver um _software_ de qualidade.

- **Lógica**: a lógica é uma disciplina fundamental para a programação de _software_. Ela trata do estudo dos princípios que regem o raciocínio correto e consistente, permitindo a criação de algoritmos e estruturas de dados que solucionem problemas de forma eficiente e elegante. A lógica está presente em diversas áreas da programação, desde a análise de requisitos até a implementação de algoritmos complexos, e é um conhecimento essencial para o desenvolvimento de _software_ de qualidade.

### A Ciência

A ciência do _Craftman_ é fundamentada em três pilares essenciais para o desenvolvimento de _software_: O Ciclo da Vida e Tomates, Construir para Durar e Pergaminhos.

- **O Ciclo da Vida e Tomates**: _circle of life_ e _pomodoro_ são duas abordagens poderosas para aumentar a produtividade e alcançar objetivos de maneira eficiente e saudável. A combinação dessas técnicas não só ajuda a gerenciar melhor o tempo e o trabalho, mas também promove o bem-estar, equilibrando o esforço com momentos de descanso, o que leva a melhores resultados e uma sensação de satisfação tanto pessoal quanto profissional.

- **Construir para Durar**: _clean design_ é uma metodologia criada pelo autor _Robert C. Martin_, também conhecido como _Uncle Bob_, que prioriza a clareza, simplicidade e facilidade de manutenção do código em todas as fases do processo de desenvolvimento de _software_. Esses princípios ajudam a criar sistemas mais eficientes e sustentáveis.

- **Pergaminhos**: _scrolls_ são um conjunto de conhecimentos e experiências que têm sido utilizados e aprimorados por desenvolvedores de _software_ ao longo dos anos, na forma de práticas, princípios e padrões. Assim como a técnica de anotações, em que ideias e _insights_ são constantemente revisados, atualizados e compartilhados, os Pergaminhos refletem o aprimoramento contínuo dessas práticas, à medida que novas experiências e aprendizados são incorporados.

## Capítulos

- [Capa](cover.md 'Capa')
- [Introdução](readme.md 'Introdução')
- [Fundamentos](foundations/readme.md 'Fundamentos')
- [Práticas Essenciais](essential-practices/readme.md 'Práticas Essenciais')
- [Pergaminhos](scrolls/readme.md 'Pergaminhos')
- Metodologia
- Conclusão
- [Referências](references.md 'Referências')

## Por onde começar?

Após a leitura da introdução, você deve estar peguntando: por onde começar?

Simples, começe pelo capítulo [**Fundamentos**](foundations/readme.md 'fundamentos').

## Notas de Atualização

Para acessar a versão anterior do livro, consulte a `branch old`.

Este livro está em desenvolvimento e, como qualquer projeto em andamento, pode apresentar erros ou imprecisões. Estamos comprometidos em corrigir esses pontos nas próximas versões.

### Previsão para Fevereiro de 2025

A versão FEV/25 será composta por:

- incremento do capítulo de fundamentos; e
- revisão do capítulo referências.

obs.: a atualização será realizada no dia 28/02/2025.

### Data da Atualização

31/01/2025
