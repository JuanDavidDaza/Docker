Clase#5
===

**27/07/2021**

Colocar a correr Jenkins
===
docker-compose -f docker-compose-jenkins.yml up -d


    docker image ls 
    docker image rmi "id"
    
    docker logs -f "nombre del contenedor"    Nos muestra si está ejecutando
    
    docker exec -it "nombre"    puedo entrar a la base de datos
    
    

**Comprimir image**

    docker save "nombre" > fedesoft-web.tar
    docker load < fedesoft-web.tar

**Limpiar el sistema Docker**

    docker system prune -all


