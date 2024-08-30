# Docker-Vite-Node-Express-Template

**Docker-Vite-Node-Express-Template** es una plantilla de Docker para un proyecto full stack. Utiliza Docker para facilitar la configuración y el desarrollo de aplicaciones. Este proyecto incluye un backend con Node.js y Express (JavaScript Vanilla) y un frontend con Vite y TSX.

## Requisitos

- Docker instalado
- Node.js v20 instalado

## Estructura del Proyecto

La estructura del proyecto se organiza en dos carpetas principales:

- **`frontend`**: Contiene la aplicación frontend construida con Vite y TSX.
- **`backend`**: Contiene la aplicación backend construida con Node.js y Express.

### Docker

El proyecto utiliza Docker para contenerizar tanto el frontend como el backend. El archivo `docker-compose.yml` está configurado para leer los `Dockerfile` de cada carpeta y levantar ambos servicios de manera independiente.

## Instrucciones de Uso

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/arceprogramando/FullStack-Vite-Node-Express-Template
   cd FullStack-Vite-Node-Express-Template
   ```
2. **Construye las imágenes y levanta los contenedores:**
    ```bash
    sudo docker-compose up --build
    ```
 **Esto construirá las imágenes de Docker para el frontend y el backend, y levantará los contenedores.**

3. **Accede a las aplicaciones**

- **`Frontend`**: http://localhost:5173
- **`Backend`**: http://localhost:8080

4. **Instalación de dependencias en entornos locales**

   Aunque la aplicación esté ejecutándose correctamente en Docker, es importante instalar las dependencias en el entorno local para evitar problemas de compatibilidad o ejecución. Para hacerlo:

   1. **Accede al directorio del frontend** y ejecuta el comando para instalar las dependencias:

      ```bash
      cd Frontend
      npm install
      ```

   2. **Accede al directorio del backend** y ejecuta el comando para instalar las dependencias:

      ```bash
      cd Backend
      npm install
      ```

   Esto asegura que tanto el frontend como el backend tengan las mismas dependencias instaladas que las que se encuentran en el contenedor Docker, evitando discrepancias entre el entorno local y el contenedor.


## Uso
Este proyecto sirve como una plantilla rápida para iniciar futuros proyectos full stack. Puedes modificar y adaptar esta estructura según tus necesidades.

## Autor
Felipe Arce
