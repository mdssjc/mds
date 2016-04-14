# Instalação

## ECLIPSE

**Objetivo:**
    Realizar a instalação do Eclipse, utilizando o arquivo eclipse-java-mars-R-linux-gtk-x86_64.

Faça o download do eclipse:
```
  wget <url>eclipse-java-mars-R-linux-gtk-x86_64
```
Descompacte o arquivo para o local /opt:
``` 
  sudo mkdir /opt/eclipse
  sudo tar -xzf eclipse-java-mars-R-linux-gtk-x86_64.tar.gz -C /opt/eclipse
```



### No Debian:

Instale o comando no sistema:
```
  sudo update-alternatives --install /usr/bin/eclipse eclipse /opt/eclipse/eclipse/eclipse 1
```
Selecione a versão do eclipse, caso exista várias:
```
  sudo update-alternatives --config eclipse
```
