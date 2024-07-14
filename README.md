# 📋 CatalogoPeliculasApp

## 📖 Descripción
CatalogoPeliculasApp es una aplicación de consola para gestionar un catálogo de películas. Permite agregar, listar y buscar películas, y almacena la información en un archivo de texto.

## 🌟 Características
- 🎬 **Agregar Película**: Añade una nueva película al catálogo proporcionando su nombre.
- 📜 **Listar Películas**: Muestra todas las películas en el catálogo.
- 🔍 **Buscar Película**: Busca una película específica en el catálogo.
- 🚪 **Salir**: Opción para salir de la aplicación.

## 📝 Código Principal

### 📂 Pelicula.java
Define una clase `Pelicula` con los siguientes atributos y métodos:
- **Atributos**: `nombre`
- **Métodos**:
  - Constructores: uno vacío y otro con el parámetro `nombre`
  - Getters y Setters para el atributo `nombre`
  - `equals()` y `hashCode()`: para comparar objetos `Pelicula`
  - `toString()`: para una representación en cadena del objeto `Pelicula`

### 📂 IServicioPeliculas.java
Define una interfaz `IServicioPeliculas` con los siguientes métodos:
- `listarPeliculas()`: Lista todas las películas.
- `agregarPelicula(Pelicula pelicula)`: Agrega una nueva película.
- `buscarPelicula(Pelicula pelicula)`: Busca una película específica.

### 📂 ServicioPeliculasArchivo.java
Implementa `IServicioPeliculas` para gestionar películas en un archivo de texto:
- **Atributos**: `NOMBRE_ARCHIVO`
- **Métodos**:
  - `listarPeliculas()`: Lista las películas leyendo del archivo.
  - `agregarPelicula(Pelicula pelicula)`: Agrega una película al archivo.
  - `buscarPelicula(Pelicula pelicula)`: Busca una película en el archivo.

### 📂 ServicioPeliculasLista.java
Implementa `IServicioPeliculas` para gestionar películas en memoria utilizando una lista:
- **Atributos**: `peliculas`
- **Métodos**:
  - `listarPeliculas()`: Lista las películas en la lista.
  - `agregarPelicula(Pelicula pelicula)`: Agrega una película a la lista.
  - `buscarPelicula(Pelicula pelicula)`: Busca una película en la lista.

### 📂 CatalogoPeliculasApp.java
Define la clase principal que gestiona la interacción con el usuario:
- **Menú Principal**:
  1. Agregar película
  2. Listar películas
  3. Buscar película
  4. Salir
- **Métodos**:
  - `mostrarMenu()`: Muestra el menú principal.
  - `ejecutarOpciones(Scanner consola, IServicioPeliculas servicioPeliculas)`: Ejecuta la operación seleccionada del menú.

## ⚙️ Requisitos
- Java 8 o superior
- IDE recomendado: IntelliJ IDEA o Eclipse

## 🚀 Ejecución
1. Clona el repositorio:
   ```bash
   git clone https://github.com/Martincho83/CatalogoPeliculasApp.git
2. Importa el proyecto en tu IDE preferido.
3. Ejecuta la clase `CatalogoPeliculasApp` para iniciar la aplicación.

## 🤝 Contribuciones
Si deseas contribuir a este proyecto, por favor realiza un fork del repositorio y crea un pull request con tus cambios.

## 👨‍💻 Autor
Martín - Desarrollador Principal - [Martincho83](https://github.com/Martincho83)

