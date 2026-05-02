# CineK — Proyecto Final TIC II

## Descripción general

**CineK** es una página web de temática cinematográfica desarrollada como proyecto final para la asignatura de **TIC II de 2º de Bachillerato**.

El proyecto simula la web de un cine, con distintas secciones dedicadas a la cartelera, estrenos y tráileres. La página combina contenido diseñado manualmente con información obtenida mediante la API de **The Movie Database \(TMDB\)**, lo que permite mostrar películas actuales, imágenes, puntuaciones y vídeos de forma dinámica.

La web está desarrollada con tecnologías frontend: **HTML, CSS y JavaScript**.

---

## Objetivos del proyecto

Los objetivos principales del proyecto son:

1. Crear una página web funcional sobre un cine ficticio.
2. Organizar el contenido en varias páginas conectadas entre sí.
3. Diseñar una interfaz visual coherente con la temática del cine.
4. Utilizar JavaScript para añadir interactividad y contenido dinámico.
5. Conectar la web con una API externa para obtener información real de películas.
6. Mostrar estrenos recientes, próximos estrenos y tráileres de forma automática.

---

## Tecnologías utilizadas

### HTML

HTML se utiliza para estructurar las distintas páginas del sitio web. Cada archivo contiene las secciones principales de la página, los menús de navegación, los contenedores de contenido y los elementos necesarios para mostrar películas, imágenes y vídeos.

### CSS

CSS se encarga del diseño visual de la web. Se utiliza para definir colores, tipografías, distribución de elementos, tarjetas de películas, botones, menús, efectos visuales y adaptación básica a distintos tamaños de pantalla.

El diseño mantiene una estética oscura y visual, relacionada con el ambiente de una página de cine.

### JavaScript

JavaScript se utiliza para añadir la parte dinámica del proyecto. Su función principal es realizar peticiones a la API de TMDB, recibir los datos en formato JSON y mostrarlos dentro de la página mediante elementos HTML generados automáticamente.

También se usa para cargar tráileres, insertar reproductores de vídeo y controlar qué información se muestra cuando una película no tiene todos los datos disponibles.

---

## API utilizada: TMDB

El proyecto utiliza la API de **The Movie Database \(TMDB\)** para obtener información actualizada sobre películas.

A través de esta API se obtienen datos como:

- Título de la película.
- Póster.
- Fecha de estreno.
- Valoración media.
- Descripción.
- Popularidad.
- Vídeos y tráileres asociados.

La API se usa principalmente en las páginas de  **cartelera**, **estrenos** y **tráileres**, donde el contenido se carga automáticamente desde JavaScript.

---

## Secciones de la web

### Inicio

La página de inicio presenta el sitio web y sirve como entrada principal a CineK. Incluye elementos visuales relacionados con el cine y accesos a las secciones principales.

### Cartelera

La cartelera muestra películas destacadas mediante tarjetas visuales. Cada tarjeta puede incluir imagen, título, breve información y botones de acceso a más contenido.

### Estrenos

La página de estrenos se divide en dos categorías:

1. **Estrenos recientes**: películas que han salido hace poco.
2. **Próximos estrenos**: películas que se estrenarán próximamente.

Los datos se cargan desde TMDB y se muestran con información como póster, título, fecha de estreno, puntuación y descripción cuando está disponible.

### Tráileres

La sección de tráileres muestra vídeos relacionados con películas recientes y próximos estrenos. Cuando TMDB proporciona un tráiler válido, se inserta un reproductor de YouTube directamente en la página.

---

## Funcionamiento de la conexión con TMDB

El funcionamiento general es el siguiente:

1. JavaScript realiza una petición a la API de TMDB.
2. TMDB devuelve una respuesta en formato JSON.
3. El código selecciona los datos necesarios de cada película.
4. Se crean tarjetas o bloques de contenido con esa información.
5. El contenido se inserta automáticamente en el HTML.
6. En la sección de tráileres, se realiza una petición adicional para obtener los vídeos de cada película.

Flujo básico:

```txt
HTML → JavaScript → API TMDB → JSON → contenido dinámico en la página
```

---

## Gestión de errores

El proyecto tiene en cuenta que no todas las películas tienen la misma cantidad de información disponible en TMDB.

Por ese motivo, algunas tarjetas pueden omitir ciertos datos si no existen, como:

- Póster.
- Puntuación.
- Descripción.
- Tráiler.

Esto evita que se muestren elementos incompletos o reproductores vacíos.


---

## Posibles mejoras futuras

Algunas mejoras que podrían añadirse son:

- Buscador de películas.
- Filtros por género.
- Página individual para cada película.
- Sistema de favoritos con `localStorage`.
- Diseño responsive más completo.
- Simulación de reserva o compra de entradas.
- Información adicional como reparto, duración o clasificación por edad.

---

## Aprendizajes del proyecto

Durante el desarrollo de CineK se han trabajado contenidos importantes de desarrollo web:

- Estructuración de páginas con HTML.
- Diseño visual con CSS.
- Organización de una web multipágina.
- Manipulación del DOM con JavaScript.
- Uso de APIs externas.
- Tratamiento de datos en formato JSON.
- Inserción dinámica de contenido.
- Integración de vídeos externos.
- Control básico de errores en contenido dinámico.

---

## Autor

Proyecto realizado por **James Berdejo Sánchez** para la asignatura de **TIC II — 2º de Bachillerato**.