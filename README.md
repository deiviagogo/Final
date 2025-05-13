### Proyecto Final Docker
## Autor: Samuel Parra Cadavid
## Descripción

Este proyecto consiste en una aplicación web ligera y escalable desarrollada con Python y Flask, empaquetada en un contenedor Docker. La aplicación sirve como una demostración práctica de los conocimientos adquiridos en el curso de Telemática, destacando el uso de contenedores para el despliegue de servicios web.
##  Tecnologías Utilizadas

- **Lenguaje:** Python 3.10
- **Framework:** Flask
- **Contenerización:** Docker
- **Frontend:** HTML5, CSS3 (estilizado incluido en index.html)
- **Sistema Operativo Base:** Ubuntu 22.04
- **Infraestructura:** Aws Ec2
- **Repositorio:** Git Hub

## 💡Requisitos

Tener -**Docker** instalado

Tener -**Git**  instalado

## 🗃️ Estructura Del Proyecto
<div style="display: flex; gap: 10px;">
    <img src="https://i.imgur.com/Gu0Wiyj.png" alt="Captura de la app" width="300"/>
    <img src="https://i.imgur.com/liisb4c.png" alt="Captura de la app 2" width="300"/>
    <img src="https://i.imgur.com/j72Zbx2.png" alt="Captura de la app 3" width="300"/>
</div>


## 🔧Instrucciones De Despliegue:
## Instalación

## 1. hacemos primero un update:
```bash
sudo apt update
```
## 2.instalamos el docker:
```bash
sudo apt install docker-compose -y
```

## 3. Clonamos este repositorio en tu maquina local:
```bash
git clone https://github.com/samuel2524/Proyecto-final.git
```

## 4. Entramos a Proyecto-final/
```bash
cd Proyecto-final/
```

## 5. Construye la imagen Docker con el siguiente comando(v01,v02,v03,v04):
```bash
sudo docker build -t proyectotelematica:1 .

```

## 6. Ejecutar el Contenedor:

```bash
sudo docker run -d -p 80:80 proyectotelematica:1
```

## 7. Verificamos si se creo

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


## tenemos que detener el contenedor anterior
```bash
docker stop container id
```

## Luego se borra
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
