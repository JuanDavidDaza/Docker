Clase 2 - Instalación
===
**21/07/2021**


En esta clase comenzamos con la instalación y realizando los comandos necesarios para adecuar nuestro ambiente en ubunto

**Link de instalación de Docker** https://docs.docker.com/engine/install/ubuntu/

| Comandos                                                                                | Función                                                                                                     |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| sudo apt-get update                                                                     | Actualizar ubuntu                                                                                           |
| sudo apt-get install \ apt-transport-https \ ca-certificates \curl \ gnupg \lsb-release | Actualice el aptíndice de paquetes e instale paquetes para permitir el aptuso de un repositorio sobre HTTPS |
| curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg                                                                                        |   Agregue la clave GPG oficial de Docker                                                                                                          |


4.  echo \
      "deb [arch=amd64 signed-by=/usr/share/keyrings /docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
  
    5.   sudo apt-get update 
    5.1. sudo apt-get install docker-ce docker-ce-cli containerd.io
    6.   sudo docker run hello-world

Instalación de Docker-container
===

**Link de instalación** https://docs.docker.com/compose/install/

    1.sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    2.sudo chmod +x /usr/local/bin/docker-compose
    3.sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
    4.docker-compose --version
    
Comandos vistos
===


| Comando                                  | función                                                      |
| ---------------------------------------- | ------------------------------------------------------------ |
| Sudo Systemctl stop docker               | Apagar servicio de Docker                                    |
| Sudo docker ps                           | Listar docker                                                |
| sudo systemctl enable docker             | Inicializa docker                                            |
| sudo systemctl status docker             | Muestra el estado                                            |
| Sudo usermod -aG docker juan             | Modificar y agregar el usuario al grupo secundario de docker |
| Docker --help                            | Comando para obtener ayuda de comandos de docker             |
| Docker ps  - Docker container ls         | Listar contenedores                                          |
| Docker image ls                          | Lista las imágenes                                           |
| Docker network ls                        | Muestra las redes                                            |
| docker container stop codimd_codimd_1    | Stop container docker                                        |
| Docker container start "id" o "nombre"   | Inicializar contenedor                                       |
| docker ps -a                             | Muestra los container en estado stop                         |
| docker container restart codimd_codimd_1 |                                                              |
| docker logs -f codimd_codimd_1            |                                                              |
|                                          |                                                              |
