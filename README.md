# Crear servicio para bd de MySql

Hola :P en primer lugar para levantar el servicio debes tener instalado Docker.

Instalar docker en linux es muy fácil. Tan sólo debes realizar los siguientes pasos:

## Instalar Docker en Linux:

1. sudo apt update

2. apt install apt-transport-https ca-certificates curl software-properties-common

3. curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

4. sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"

5. sudo apt install docker-ce

6. sudo systemctl status docker or sudo systemctl restart docker

## Instalar Docker en Windwos

Vídeo recomendado: https://www.youtube.com/watch?v=_et7H0EQ8fY&pp=ygUZaW5zdGFsYXIgZG9ja2VyIG53IGRpbndvcw%3D%3D

Una vez teniendo docker es tan sencillo como irse a la carpeta docker-compose-mysql

Editar el archivo docker-compose.yml y colocar el nombre de base de datos que quieras.

En caso de control de despacho puedes colocar "dispatch_control" o "visits_control" guardar los cambios >

ejecutar:

```sh
docker compose up -d
```

Para ingresar al gestor de base de datos PHPMyAdmin ir al navegador preferido:

en url colocar:

localhost:8081 

el usuario es: `user`
y la clave es: `pass1234`


Para crear un diseño de la base de datos ir a la pestaña diseños en phpmyadmin