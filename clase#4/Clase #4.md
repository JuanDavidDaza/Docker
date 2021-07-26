Clase #4
===
**26/07/2021**

Archivo docker-compose
=

**Volumes**: dirección del directorio dentro del host 
Nos va poder servir para la comunicación de los servicios de docker 

Entrar al editor de texto MD
=
	docker-compose up -d 
	ip:3000
	ej:
	http://192.168.1.102:3000/



| Comandos                                         | Función                          |
| ------------------------------------------------ | -------------------------------- |
| free -h                                          | Muestra los recursos del sistema |
| docker-compose up --scale web=5 -d               |                                  |
| docker stop "id"                                 | detener un contenedor            |
| docker container rm "id"                         | Elimina un contenedor            |
| docker-compose -f "nombre del archivo".yml up -d |                                  |
**Diferencia entre un contenedor y una imagen:**
    El contenedor es el recipiente en el que puedo prender, apagar, etc.
    Imagen es como el sistema operativo


Instación de Jenkins **"Super Importante"**
===


    cd Jenkins/
    docker-compose -f docker-compose-jenkins.yml up -d
    sudo chown juan:juan jenkins_home/	 "Importante dar permisos a la carpeta sino no va funcionar"
    sudo chmod 2777 jenkins_home/
    docker logs -f jenkins

    Logear por la ip:8090
    Colocar la contraseña de dan en consola 
    Despues instalar los plugin 
    Crear un usuario y contraseña 
    
        Usuario: juan
        Contraseña: juan
        http://192.168.1.102:8090/
