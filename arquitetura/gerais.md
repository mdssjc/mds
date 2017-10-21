# Gerais

* [**_Execute Around Method_**](http://wiki.c2.com/?ExecuteAroundMethod "Execute Around Method"): controle sobre recursos externos, como operações em _cleanup_ e _locks_.

* [**Princípio de _Hollywood_**](http://wiki.c2.com/?HollywoodPrinciple "Hollywood Principle") - _Hollywood Principle_: Não nos chame, nós chamaremos você - _Don't call us, we will call you_, especifica como componentes de alto e baixo nível interagem sem criar dependências, sendo uma técnica para a construção de _frameworks_ e componentes.

* [**Ordene, não peça!**](http://wiki.c2.com/?TellDontAsk "Tell, don't ask!") - _Tell, don't ask!_: peça o produto da informação ao elemento de programação na qual é dono da informação - reduza os acoplamentos, priorizando o encapsulamento.

  Técnica para refatoração: redirecionamento e delegação

* [**Princípio do Mínimo Conhecimento**](http://wiki.c2.com/?LawOfDemeter "Principle of Least Knowledge") - _Principle of Least Knowledge_: também conhecido por _Law of Demeter_ (1988) ou _Don't Talk to Strangers_, fale somente com seus amigos imediatos:

  1. O elemento em si;
  2. Os elementos passados como parâmetros para o elemento;
  3. Quaisquer elementos criados e/ou instanciados;
  4. Quaisquer componentes do elemento; e
  5. Os elementos globais.
