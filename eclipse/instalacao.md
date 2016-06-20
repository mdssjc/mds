# Instalação
**Objetivo**: realizar a instalação do *software* *Eclipse*.

Faça o *download* do *Eclipse*:
```
  wget <url>/<file>.tar
```
Descompacte o arquivo para o local ```/opt```:
``` 
  sudo mkdir /opt/eclipse
  sudo tar -xzf <file>.tar -C /opt/eclipse
```
Execute o arquivo ```eclipse```:
```
  cd /opt/eclipse
  eclipse
```

## No Arch Linux
No arquivo ```eclipse.ini```, inclua o seguinte parâmetro em ```org.eclipse.platform```:
```
  org.eclipse.platform
  --launcher.GTK_version
  2
```

[https://wiki.archlinux.org/index.php/eclipse](https://wiki.archlinux.org/index.php/eclipse)
