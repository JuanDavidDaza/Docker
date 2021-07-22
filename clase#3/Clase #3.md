Clase #3
===
**22/07/2021**

**Imágenes:** una imagen es una plantilla de solo lectura con instrucciones.

Para crear su propia imagen, cree un Dockerfile con una sintaxis simple para definir los pasos necesarios para crear la imagen.

    link de docker nginx https://hub.docker.com/_/nginx



| Comando                                                       | Función                                                    |
| ------------------------------------------------------------- | ---------------------------------------------------------- |
| docker info                                                   | muestra toda la información relacionada con Docker         |
| Docker version                                                | Nos saca las versiones que maneja                          |
| Docker image rmi "id"                                         | Eliminar la imagen                                         |
| docker run --name some-nginx -d -p 8080:80 some-content-nginx | Correr el contenedor                                       |
| Docker logs -f "nombre del contenedor"                        | Buscar algún problema o mirar el estado                    |
| docker run --name some-nginx -d -p 8080:80 some-content-nginx | Queda con el nombre some-nginx                             |
| Curl -k localhost:8080                                        | La opción -k es para que no me mire la seguridad           |
| docker inspect "nombre del contenedor"                        | Nos muestra toda la información referente a ese contenedor |
| Docker stats "nombre del contenedor"                          | Muestra la memoria que está utilizando                     |

    Docker commit https://docs.docker.com/engine/reference/commandline/commit/
    
Usuario: juandaviddaza


| Docker Login                                                  | Iniciar sección       |
| ------------------------------------------------------------- | --------------------- |
| sudo docker tag some-content-nginx juandaviddaza/fedesoft-web | Tag al contenedor     |
| sudo docker push juandaviddaza/fedesoft-web                   | Subirlo al contenedor |

    Link del repositorio en Docker https://hub.docker.com/r/juandaviddaza/fedesoft-web/tags?page=1&ordering=last_updated
    con el ejercicio subido





