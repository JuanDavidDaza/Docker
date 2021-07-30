Clase#6
===
**28/07/2021**

Agregar credenciales a Jenkins
===
    hacer la conexión ssh por medio del programa Moba
    mirar la ip de la maquina virtual con "ip a s"
    conectarse por Moba con "ssh ip -l usuario"
    
    por medio de la ip abrir el navegador y entrar con la ip:8090
    para entrar a Jenkins
    
    Buscar opción Add Credentials
    
    pass: la que genera la consola 
    

Herramienta django
===
     1.Cree un directorio de proyecto vacío. 
     Puede nombrar el directorio con algo fácil de recordar. 
     Este directorio es el contexto de la imagen de su aplicación. 
     El directorio solo debe contener recursos para construir esa imagen.
     
     2.Crea un nuevo archivo llamado Dockerfile en el directorio de tu proyecto. 
     El Dockerfile define el contenido de la imagen de una aplicación a través
     de uno o más comandos de compilación que configuran esa imagen.
     Una vez construida, puede ejecutar la imagen en un contenedor. 
     Para obtener más información sobre Dockerfile.
     
     
     3.Agregue el siguiente contenido al Dockerfile.
     
     
        FROM python:3

        ENV PYTHONUNBUFFERED=1
        WORKDIR /code
        COPY requirements.txt /code/
        RUN pip install -r requirements.txt
        COPY . /code/
        
        guardar y salir ":wq"
        
    4. RUN pip install -r requirements.txt


        
     

**Link de documentación usada** https://github.com/jsgiraldoh/Django-postgres

**GitHub del Profesor** 
https://github.com/jsgiraldoh