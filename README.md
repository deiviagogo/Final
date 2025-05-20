### Proyecto Final Docker
## Autor: David Vallejo Garcia
## Descripción

Este proyecto es una aplicación web simple y fácil de ampliar, hecha con Python y Flask, y que se ejecuta dentro de un contenedor Docker. Sirve como ejemplo práctico de lo aprendido en el curso de Telemática, mostrando cómo usar contenedores para poner en marcha servicios web.

##  Herramientas y Tecnologías Empleadas
Python 3.10 como lenguaje principal de desarrollo.

Flask, un microframework ligero para la creación de aplicaciones web.

Docker para contenerizar y facilitar el despliegue de la aplicación.

HTML5 y CSS3, integrados directamente en el archivo index.html, para el diseño de la interfaz.

Ubuntu 22.04 como sistema operativo base en el entorno de ejecución.

Amazon EC2 (AWS) como plataforma para la infraestructura en la nube.

GitHub para el control de versiones y alojamiento del código fuente.

## 💡Requisitos

Tener -**Docker** instalado

Tener -**Git**  instalado

## 🔧Instrucciones De Despliegue:
## Instalación

## 1. Utilizamos un update:
```bash
sudo apt update
```
## 2.instalamos el docker:
```bash
sudo apt install docker-compose -y
```

## 3. Clonamos el siguiente repositorio en nuestra maquina local:
```bash
git clone https://github.com/deiviagogo/Final
```

## 4. Entramos a Final/
```bash
cd Final/
```

## 5. Construye la imagen Docker con el siguiente comando(v01,v02,v03,v04):
```bash
sudo docker build -t proyectotelematica:1 .

```

## 6. Ejecutar el Contenedor:

```bash
sudo docker run -d -p 80:80 proyectotelematica:1
```

## 7. Verificamos si esta creado

```bash
sudo docker ps
```
## 8. Acceder a la Aplicación con la ip publica

```bash
http://ip publica
```

## 🛠️ ¿Cómo Modificar?

- **Modifica el contenido o diseño fácilmente editando los siguientes archivos:**

    - **app/templates/index.html: Cambia el contenido HTML de la página.**


## Detenemos el contenedor anterior
```bash
docker stop container id
```

## Luego se elimina
```bash
docker rm container id
```
## Reconstruir la imagen:

```bash
sudo docker build -t proyectotelematica:1 .
```
## Volvemos A Ejecutar El Contenedor:

```bash
sudo docker run -d -p 80:80 proyectotelematica:1
```
