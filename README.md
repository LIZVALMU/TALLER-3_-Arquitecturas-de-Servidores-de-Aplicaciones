# Taller 3  Arquitecturas de Servidores de Aplicaciones

[![Java](https://img.shields.io/badge/Java-21-orange.svg)](https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html)
[![Maven](https://img.shields.io/badge/Maven-3.x-blue.svg)](https://maven.apache.org/)
![HTTP](https://img.shields.io/badge/HTTP-1.1-blue) |
![JSON](https://img.shields.io/badge/JSON-Supported-green?logo=json&logoColor=white) 

## Introducción

El objetivo fue extender las capacidades para soportar servicios REST y así permitir la creación de aplicaciones web más completas.

El framework permite

- Definir rutas con funciones lambda utilizando el método **get().**
- Extraer parámetros de consulta de las solicitudes 
- Configurar la ubicación de archivos estáticos **staticfiles()**
---

## Tecnologías Utilizadas

| Tecnología      | Versión       | Propósito                   |
|-----------------|---------------|-----------------------------|
| Java            | 21            | Desarrollo backend          |
| Sockets         | Java Nativo   | Comunicación de red         |
| HTTP/1.1        | -             | Implementación de protocolo |
| JSON            | Nativo        | Respuestas API              |

---

## Instalación

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/LIZVALMU/TALLER-3_-Arquitecturas-de-Servidores-de-Aplicaciones.git
   ```

2. Compilar el proyecto (Maven):
   ```bash
   mvn clean package
   ```

3. Asegurarse de tener instalado:
   - **Java 21**
   - **Maven 3.x**

---

## Ejecución

1. Ingresar a la carpeta 
    ```bash
   cd taller2_arep
   ```
2. Instalar las dependencias
    ```bash
   mvn clean compile
   ```
3. Ejecutar el servidor:
   ```bash
      java -cp target/classes escuela.edu.co.HttpServer
   ```

**si desea especificar un puerto diferente, puede hacerlo al iniciar el servidor:**

```bash
   java -cp target/classes escuela.edu.co.HttpServer <puerto>
```

4. Abrir en un navegador:
   ```
   http://localhost:35000/index.html
   ```

   > El servidor por defecto corre en el puerto `35000`.  

5. Para probar los servicios REST (ejemplo):
   - GET: `http://localhost:35000/hello?name=Alison`
   - POST: `http://localhost:35000/hellopost?name=Alison`

---

## Arquitectura del Prototipo

El sistema está compuesto por tres módulos principales:


---

## Evaluación (Pruebas Realizadas)


---

## Project Structure

```bash
arep_httpserver/
├── src/
│   └── main/
│       └── java/
│           └── escuela/
│               └── edu/
│                   └── co/
│                       └── HttpServer.java    # Servidor HTTP principal
└── www/                                        # Archivos estáticos
    ├── index.html                             # Página principal
    ├── app.js                                 # JavaScript frontend
    ├── style.css                              # Estilos CSS
    └── logo.png                               # Recursos multimedia
```
---

## Autor

- [Alison Geraldine Valderrama Munar](https://github.com/alisongvalderrama)

## License
Este proyecto está licenciado bajo la MIT License
