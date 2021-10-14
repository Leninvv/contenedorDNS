# Descripción Docker-compose.yml

## **Version**
    En este apartado definimos la versión a utilizar del docker-compose.

## **Services**
    En este apartado definimos los servicios a crear, cada servicio comienza escribiendo su nombre seguido de dos puntos. E.g. primer_servicio:

### **- Image**
    Introducimos la imagen y versión a utilizar en el servicio.

### **- Ports**
    Aquí definimos la sincronización de puertos entre el contenedor y nuestra máquina, siendo los puertos de la izquierda los de la máquina y los de la derecha los del contenedor.

### **- Volumes**
    Aquí definimos los volúmenes a utilizar, estos pueden ser creados por el docker o puede usar un directorio del host. Para usar un directorio del host introducimos la ruta dentro de la máquina, para que el docker cree un volumen simplemente introducimos el nombre del mismo sin ninguna ruta.

## **Volumes**
    No confundir con el subapartado de Services, en este apartado definimos los volúmenes no vinculados a una ruta del host, es decir, definimos los volúmenes que va a crear el docker una vez ejecutemos el docker-compose. Para definir los volúmenes introducimos el nombre que le dimos previamente seguido de dos puntos y la definición. Si la definición está vacía se creará un volumen con la configuración por defecto. E.g. volumen_1: definición.