Claro, he reestructurado y mejorado tu archivo `README.md` para que sea más claro, profesional y completo.

A continuación, te presento la versión mejorada. Puedes copiar el texto directamente o descargar el archivo `.md` al final.

-----

# Servidor de Aplicaciones Web con API REST en Java

Un servidor de aplicaciones web ligero y extensible construido en Java 21, diseñado para manejar solicitudes HTTP, servir archivos estáticos y exponer servicios RESTful.

[](https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html)
[](https://maven.apache.org/)
[](https://www.google.com/search?q=%5Bhttps://opensource.org/licenses/MIT%5D\(https://opensource.org/licenses/MIT\))

-----

## Introducción

Este proyecto presenta un servidor de aplicaciones web desarrollado desde cero en Java utilizando Sockets nativos. El objetivo principal fue construir una base sólida para entender el funcionamiento interno de los servidores web y, posteriormente, extender sus capacidades para soportar una API REST.

El framework resultante es capaz de servir contenido estático (HTML, CSS, JavaScript) y de definir dinámicamente *endpoints* para servicios web, permitiendo la creación de aplicaciones web interactivas y completas.

-----

## ✨ Características Principales

  - **Servidor HTTP/1.1:** Implementación del protocolo para manejar solicitudes `GET` y `POST`.
  - **Enrutamiento Dinámico:** Define rutas para servicios REST de manera programática utilizando funciones lambda con el método `get()`.
  - **Manejo de Archivos Estáticos:** Configura un directorio (`/www` por defecto) para servir archivos como HTML, CSS, JS e imágenes.
  - **Procesamiento de Parámetros:** Extrae fácilmente parámetros de la *query string* en las solicitudes HTTP.
  - **Respuestas en JSON:** Capacidad nativa para formular y enviar respuestas en formato JSON, ideal para APIs.

-----

## 🛠️ Tecnologías Utilizadas

| Tecnología | Versión | Propósito |
| :--- | :--- | :--- |
| **Java** | 21 | Lenguaje principal para el desarrollo de toda la lógica del backend. |
| **Sockets Nativos**| Java Native | Utilizados para la comunicación de red de bajo nivel, gestionando la conexión TCP/IP. |
| **HTTP/1.1** | - | Implementación del protocolo estándar para la comunicación cliente-servidor. |
| **JSON Nativo** | - | Formateo manual de respuestas de la API, sin dependencias externas. |
| **Maven** | 3.9+ | Gestión de dependencias del proyecto, compilación y empaquetado. |

-----

## 🚀 Instalación y Ejecución

Sigue estos pasos para poner en marcha el servidor en tu entorno local.

### Prerrequisitos

Asegúrate de tener instalado lo siguiente en tu sistema:

  * **Java 21** (JDK)
  * **Maven 3.9** o superior
  * **Git**

### Pasos

1.  **Clonar el repositorio:**

    ```bash
    git clone https://github.com/LIZVALMU/TALLER-3_-Arquitecturas-de-Servidores-de-Aplicaciones.git
    cd TALLER-3_-Arquitecturas-de-Servidores-de-Aplicaciones
    ```

2.  **Compilar el proyecto con Maven:**
    Este comando limpiará el proyecto, descargará las dependencias y empaquetará la aplicación.

    ```bash
    mvn clean package
    ```

3.  **Ejecutar el servidor:**
    Ejecuta el servidor desde la raíz del proyecto. Por defecto, se iniciará en el puerto `35000`.

    ```bash
    java -cp target/classes escuela.edu.co.HttpServer
    ```

    **Para usar un puerto diferente:**
    Si deseas especificar otro puerto, pásalo como argumento al ejecutar el comando.

    ```bash
    java -cp target/classes escuela.edu.co.HttpServer 8080
    ```

4.  **Acceder a la aplicación:**
    Abre tu navegador web y visita la siguiente URL:
    `http://localhost:35000/index.html`

-----

## 🧪 Ejemplos de Uso (API REST)

Una vez que el servidor esté en funcionamiento, puedes probar los siguientes *endpoints*:

  * **Servicio GET:**
    `http://localhost:35000/hello?name=Alison`

  * **Servicio POST:**
    Utiliza una herramienta como Postman o `curl` para probar este endpoint.
    `http://localhost:35000/hellopost?name=Alison`

-----

## 📂 Estructura del Proyecto

```
TALLER-3_-Arquitecturas-de-Servidores-de-Aplicaciones/
├── .git/
├── src/
│   └── main/
│       └── java/
│           └── escuela/
│               └── edu/
│                   └── co/
│                       └── HttpServer.java    # Clase principal del servidor HTTP
├── www/                                       # Directorio de archivos estáticos
│   ├── index.html                             # Página de inicio
│   ├── app.js                                 # Lógica del frontend
│   ├── style.css                              # Estilos
│   └── logo.png                               # Recursos gráficos
├── pom.xml                                    # Archivo de configuración de Maven
└── README.md                                  # Archivo de documentación
```

-----

## 👤 Autor

  * **Alison Geraldine Valderrama Munar**
      * GitHub: [Alison Valderrama](https://github.com/lizvalmu)

-----

## 📜 Licencia

Este proyecto está distribuido bajo la **Licencia MIT**. Consulta el archivo `LICENSE` para más detalles.

-----

