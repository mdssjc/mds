# Emacs

![](/images/emacs-old-logo.png)

O _[Emacs](https://www.gnu.org/software/emacs/)_ é um incrível editor com total personalização, construído sobre um interpretador.

## Instalação

Clone o repositório do _Emacs_ no _Github_:

`git clone https://github.com/emacs-mirror/emacs`

Compile e instale o _Emacs_:

```
./autogen.sh all
./configure [--with-modules --enable-link-time-optimization --with-x-toolkit=gtk3 --with-xwidgets]
make
sudo make install
```

Para atualizar:

`git pull`

E repita a etapa anterior.

Informações sobre a instalação:

Arquivo `INSTALL`.

## Extensão

O _Emacs_ possui a poderosa extensão _[Spacemacs](http://spacemacs.org/)_ para os usuários que preferem um _bootstarter_.

