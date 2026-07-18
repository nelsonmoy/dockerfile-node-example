# Dockerfile Node Example

Repositorio de ejemplo utilizado en la publicación **"Docker. Uno de los archivos mágicos, el Dockerfile"**.

Este proyecto tiene como objetivo mostrar, de forma práctica, cómo construir una imagen de Docker a partir de un **Dockerfile** y ejecutar un contenedor con una aplicación sencilla desarrollada en **Node.js**.

Es un ejemplo pensado para quienes están dando sus primeros pasos con Docker y desean comprender cómo funciona el proceso de construcción de imágenes.

## 📋 Requisitos

Antes de comenzar, asegúrate de tener instalado:

* Docker
* Git

## 🚀 Clonar el repositorio

```bash
git clone https://github.com/nelsonmoy/dockerfile-node-example.git
```

Ingresa al directorio del proyecto:

```bash
cd dockerfile-node-example
```

## 🏗️ Construir la imagen

Ejecuta el siguiente comando:

```bash
docker build .
```

Durante la construcción es posible que Docker descargue automáticamente la imagen base y otros componentes necesarios. Esto es completamente normal y solo ocurrirá la primera vez.

Al finalizar, habrás construido tu primera imagen utilizando un **Dockerfile**.

## 🔎 Obtener el ID de la imagen

Para listar las imágenes disponibles ejecuta:

```bash
docker image ls
```

Obtendrás una salida similar a:

```text
REPOSITORY   TAG       IMAGE ID       CREATED          SIZE
<none>       <none>    3795230e0d7f   10 seconds ago   XX MB
```

La imagen creada más recientemente será la correspondiente a este proyecto.

## ▶️ Ejecutar el contenedor

Utiliza el **IMAGE ID** obtenido anteriormente:

```bash
docker container run 3795230e0d7f
```

Si todo salió correctamente, la aplicación mostrará en pantalla el mensaje definido en el proyecto.

## 📄 Dockerfile

El archivo `Dockerfile` incluido en este repositorio demuestra algunos de los comandos más utilizados en Docker.

```Dockerfile
FROM alpine
RUN apk update && apk add nodejs
COPY . /app
WORKDIR /app
CMD ["node", "index.js"]
```

### ¿Qué hace cada instrucción?

| Instrucción | Descripción                                                                                   |
| ----------- | --------------------------------------------------------------------------------------------- |
| `FROM`      | Define la imagen base sobre la cual se construirá la nueva imagen.                            |
| `RUN`       | Ejecuta comandos durante la construcción de la imagen, como instalar paquetes o dependencias. |
| `COPY`      | Copia los archivos del proyecto desde el equipo anfitrión hacia el contenedor.                |
| `WORKDIR`   | Establece el directorio de trabajo para las instrucciones posteriores.                        |
| `CMD`       | Define el comando que se ejecutará cuando el contenedor inicie.                               |

## 📚 Artículo relacionado

Este repositorio acompaña la publicación:

**Docker. Uno de los archivos mágicos, el Dockerfile.**

En dicho artículo se explica con mayor detalle:

* Qué es un Dockerfile.
* Cómo Docker interpreta cada instrucción.
* Cómo construir imágenes paso a paso.
* Cómo ejecutar contenedores basados en dichas imágenes.

## 🎯 Objetivo del proyecto

Este repositorio es únicamente un ejemplo educativo para aprender:

* La estructura básica de un Dockerfile.
* El proceso de construcción de imágenes.
* La ejecución de contenedores.
* El funcionamiento de las instrucciones más comunes de Docker.

---

Si este ejemplo te fue útil, no olvides darle una ⭐ al repositorio. ¡Te ayudará a que más personas encuentren este material y continúen aprendiendo Docker!
