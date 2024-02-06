# SSH
##  Acceso remoto SSH mediante clave privada
### Paso 1
Para generar una clave privada tendremos que hacer el comando:
```console
ssh-keygen -t rsa -f ~/.ssh/id_rsa
``` 
### Paso 2
Ahora copiaremos la clave al equipo al que queramos acceder con SSH
```console
ssh-copy-id -i ubicacion\del\archivo usuario@remote_host
```
### Paso 3
Ahora accederemos utilizando el siguiente comando:
```console
ssh -i clave_que_utilizaremos username@remote_host
```
# SSH keys en Github

Haremos un cat de la clave publica
```console
cat id_rsa.pub
```
y la copiaremos, después solo tendremos que acceder a configuracion, le daremos a ssh and gpg keys y le daremos a añadir una nueva ssh-key y solo nos quedaria pegarla.
