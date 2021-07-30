Clase#8
===
**30/07/2021**

Docker-Compose en linux(ubunto)
===

    sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    sudo chmod +x /usr/local/bin/docker-compose
    docker-compose --version
    
**Documentación por parte de Docker** https://docs.docker.com/compose/install/



Usar y ejecutar Docker en un disco duro externo
===
    -mkdir /media/nextcloud/docker
    -sudo service docker stop
    -sudo vim /etc/docker/daemon.json
    
        SE COPIA Y PEGA ESTE CODIGO 
        {
       "graph": "/media/nextcloud/docker"
        }
        
    -sudo rsync -aP /var/lib/docker/ /media/nextcloud/docker
    -sudo mv /var/lib/docker /var/lib/docker.old
    -sudo service docker start
    -docker info | grep Docker

Comprimir una image
===
    Docker save ubunto > ubunto.tar
    Docker load < ubunto.tar
    Y ya carga la imagen 



Comandos vistos
===
    Sudo systemctl enable docker (Importante este comando para que se inicialice docker) 
    Docker --help	(Muestra todos los comandos posibles de Docker)
    Docker image ls	(Listar imágenes)
    Docker save nginx > nginx.tar	(Empaquetar las imágenes)
    Docker image rmi "id"	(Eliminar una imagen)
    Docker rmr ""	(Eliminar)
    Docker pull ubunto	



**Link de documentación de instalar docker en otra partición** https://geekland.eu/usar-y-ejecutar-docker-en-un-disco-duro-externo/