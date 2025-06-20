Literatura API - Documentación
📚 Descripción del Proyecto
Literatura API es una aplicación Spring Boot que se integra con la API de GutenDex para buscar y mostrar información sobre libros, autores y obras literarias. La aplicación almacena los resultados en una base de datos PostgreSQL para permitir búsquedas rápidas y acceso offline a la información.

✨ Características Principales
🔍 Búsqueda de libros por título, autor o palabras clave
📖 Visualización detallada de información de libros
🗃️ Almacenamiento en caché de resultados en base de datos PostgreSQL
🔄 Sincronización periódica con GutenDex API
🚀 API RESTful para integración con otros sistemas
🛠 Tecnologías Utilizadas
Backend:

Java 11
Spring Boot 2.6.4
Spring Data JPA
Maven
Base de Datos:

PostgreSQL
APIs Externas:

GutenDex API (https://gutendex.com/)
⚙️ Configuración del Entorno
Requisitos Previos
Java JDK 11+
Maven 3.8+
PostgreSQL 12+
Variables de entorno configuradas (ver .env.example)
Instalación
Clonar el repositorio:

bash
Run
Copy code
git clone [URL_DEL_REPOSITORIO]
Configurar variables de entorno:

bash
Run
Copy code
cp .env.example .env
Editar el archivo .env con tus credenciales

Ejecutar la aplicación:

bash
Run
Copy code
mvn spring-boot:run
📡 Endpoints de la API
Libros
GET /api/books - Lista todos los libros almacenados
GET /api/books/search?query={busqueda} - Busca libros por título/autor
GET /api/books/{id} - Obtiene detalles de un libro específico
Autores
GET /api/authors - Lista todos los autores
GET /api/authors/{id} - Obtiene información de un autor específico
🏗 Estructura del Proyecto
Run
Copy code
literatura/
├── src/
│   ├── main/
│   │   ├── java/com/ccorel/proyectos/literatura/
│   │   │   ├── controller/       # Controladores API
│   │   │   ├── model/            # Entidades JPA
│   │   │   ├── repository/       # Repositorios Spring Data
│   │   │   ├── service/          # Lógica de negocio
│   │   │   └── LiteraturaApplication.java
│   │   └── resources/
│   │       ├── application.properties # Configuración
│   │       └── data/             # Datos iniciales (opcional)
├── pom.xml                       # Configuración Maven
└── README.md
🌟 Contribuciones
Las contribuciones son bienvenidas. Por favor, sigue las directrices de contribución del proyecto.

----------------------------------

# Literatura API - Documentación

## 📚 Descripción del Proyecto

Literatura API es una aplicación Spring Boot que se integra con la API de GutenDex para buscar y mostrar información sobre libros, autores y obras literarias. La aplicación almacena los resultados en una base de datos PostgreSQL para permitir búsquedas rápidas y acceso offline a la información.

## ✨ Características Principales

- 🔍 Búsqueda de libros por título, autor o palabras clave
- 📖 Visualización detallada de información de libros
- 🗃️ Almacenamiento en caché de resultados en base de datos PostgreSQL
- 🔄 Sincronización periódica con GutenDex API
- 🚀 API RESTful para integración con otros sistemas

## 🛠 Tecnologías Utilizadas

- **Backend**: 
  - Java 17
  - Spring Boot 3.3.0
  - Spring Data JPA
  - Maven

- **Base de Datos**:
  - PostgreSQL

- **APIs Externas**:
  - GutenDex API (https://gutendex.com/)

## ⚙️ Configuración del Entorno

### Requisitos Previos

- Java JDK 17+
- Maven 3.8+
- PostgreSQL 12+
- Variables de entorno configuradas (ver `.env.example`)

### Instalación

1. Clonar el repositorio:
   ```bash
   git clone [URL_DEL_REPOSITORIO]
   ```

2. Configurar variables de entorno:
   ```bash
   cp .env.example .env
   ```
   Editar el archivo `.env` con tus credenciales

3. Ejecutar la aplicación:
   ```bash
   mvn spring-boot:run
   ```

## 📡 Endpoints de la API

### Libros

- `GET /api/books` - Lista todos los libros almacenados
- `GET /api/books/search?query={busqueda}` - Busca libros por título/autor
- `GET /api/books/{id}` - Obtiene detalles de un libro específico

### Autores

- `GET /api/authors` - Lista todos los autores
- `GET /api/authors/{id}` - Obtiene información de un autor específico

## 🏗 Estructura del Proyecto

```
literatura/
├── src/
│   ├── main/
│   │   ├── java/com/ccorel/proyectos/literatura/
│   │   │   ├── controller/       # Controladores API
│   │   │   ├── model/            # Entidades JPA
│   │   │   ├── repository/       # Repositorios Spring Data
│   │   │   ├── service/          # Lógica de negocio
│   │   │   └── LiteraturaApplication.java
│   │   └── resources/
│   │       ├── application.properties # Configuración
│   │       └── data/             # Datos iniciales (opcional)
├── pom.xml                       # Configuración Maven
└── README.md
```

## 🌟 Contribuciones

Las contribuciones son bienvenidas. Por favor, sigue las directrices de contribución del proyecto.

## 📄 Licencia

Este proyecto está licenciado bajo [MIT License](LICENSE).
