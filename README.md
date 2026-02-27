Descripción del Proyecto
El proyecto consiste en una página web estática de tipo landing page o página de presentación para un evento tecnológico ficticio llamado "Jornada Tecnológica San Valero 2026". Su objetivo es informar a los asistentes potenciales sobre los detalles del evento (fecha, lugar, temática), mostrar el programa de actividades, presentar a los ponentes destacados y proporcionar un formulario de inscripción. El diseño es limpio, moderno y totalmente responsivo, lo que garantiza una correcta visualización en dispositivos móviles, tablets y ordenadores de escritorio.

Secciones Usadas y Sistema de Rejilla (Grid) de Bootstrap
La página está estructurada en varias secciones claramente diferenciadas, utilizando el sistema de rejilla de Bootstrap (basado en filas .row y columnas .col-*-*) para organizar el contenido.

Barra de Navegación (<nav>): Contiene el logo y el título a la izquierda, y los enlaces de navegación a la derecha. Se apoya en las clases navbar, navbar-expand-lg, container y ms-auto para alinear los elementos del menú.

Hero / Cabecera (#inicio): Es la sección de bienvenida.

Columnas usadas: No utiliza una rejilla compleja. El contenido está centrado dentro de un .container. Los detalles de fecha y ubicación se muestran en un contenedor flexible (.d-flex) para que se apilen en móviles.

Programa (#programa): Presenta las diferentes actividades del evento en formato de tarjetas.

Columnas usadas: Emplea una fila (.row) con una sola columna que ocupa todo el ancho para el título. Para las tarjetas, se utiliza un bucle de Bootstrap con las clases col-md-6 col-lg-4. Esto significa que en pantallas medianas (md) se mostrarán 2 columnas (6/12), y en pantallas grandes (lg) se mostrarán 3 columnas (4/12). En móviles, por defecto, se apilarán una debajo de otra.

Ponentes (#ponentes): Muestra las fotos y datos de los conferenciantes.

Columnas usadas: Similar a la sección anterior, usa una fila con la clase col-md-6 col-lg-3. Así, en pantallas medianas se ven 2 ponentes por fila y en pantallas grandes, 4 ponentes por fila (3/12 * 4 = 12/12).

Inscripción (#inscripcion): Contiene el llamado a la acción y el formulario.

Columnas usadas: Para centrar el formulario, se utiliza una fila con una columna que se centra gracias a justify-content-center. El formulario está dentro de col-lg-8 col-xl-6, lo que hace que ocupe 8/12 en pantallas grandes y 6/12 en pantallas extra grandes, manteniéndolo centrado y con un ancho adecuado.

Pie de Página (<footer>): Contiene iconos de redes sociales y la dirección de contacto. Todo está centrado dentro de un .container.

Componentes Prediseñados de Bootstrap Usados
El proyecto hace un uso extensivo de los componentes de Bootstrap para acelerar el desarrollo y mantener la coherencia visual:

Navbar (navbar, navbar-dark, navbar-expand-lg): Para crear una barra de navegación responsiva que se colapsa en dispositivos móviles.

Botones (btn, btn-primary, btn-lg, btn-dark): Para el botón de "Inscribirme gratis" en el hero y el botón de envío del formulario.

Tarjetas (card, card-body, card-title, card-text): Para mostrar de forma estructurada y atractiva cada sesión del programa y el contenido de los ponentes.

Formulario (form-control, form-select): Para los campos de entrada de texto, email, el selector desplegable y el área de texto, dándoles un estilo consistente y responsivo.

Iconos de Bootstrap Icons (bi, bi-robot, bi-calendar-event, etc.): Para añadir elementos visuales intuitivos a las tarjetas del programa, los datos del evento y las redes sociales.

Sistema de Rejilla (container, row, col-*): La base de todo el maquetado responsivo.

Clases de Utilidades (text-center, bg-light, bg-primary, text-white, shadow, d-flex, gap-4, etc.): Para un rápido ajuste de espaciado, alineación, colores y sombras sin necesidad de CSS personalizado.

Descripción de los Commits y Mejoras Implementadas
Para simular la evolución del proyecto, estos podrían ser los pasos o commits realizados:

Commit 1: Estructura inicial y contenido básico.

Se crea el esqueleto HTML5 y se enlazan los archivos CSS y JS de Bootstrap.

Se añade la barra de navegación con las secciones principales.

Se incluye el texto del Hero con el título, fecha y lugar del evento.

Se maqueta la sección de ponentes con imágenes de muestra y texto.

Se crea el pie de página con iconos de redes sociales.

Commit 2: Implementación del programa con tarjetas.

Se añade la sección #programa.

Se utiliza el componente card de Bootstrap para cada franja horaria.

Se aplican las clases de columna col-md-6 col-lg-4 para que las tarjetas se distribuyan correctamente según el tamaño de pantalla.

Se añaden iconos temáticos a cada tarjeta usando Bootstrap Icons para hacerla más visual.

Commit 3: Diseño del formulario de inscripción.

Se crea la sección #inscripcion con un fondo azul (bg-primary).

Se implementa el formulario con los campos necesarios usando las clases form-control y form-select.

Se añade la lógica de centrado con justify-content-center y se limita el ancho del formulario con col-lg-8 col-xl-6.

Se incorpora el botón de envío estilizado con btn-dark.

Commit 4: Personalización avanzada con CSS.

Se añade el bloque <style> en el <head> para aplicar estilos personalizados.

Se definen variables CSS (:root) para los colores principales.

Se estiliza la barra de navegación para que tenga un color más oscuro y una sombra.

Se crea la imagen de fondo del Hero con una capa de superposición oscura (linear-gradient).

Se diseña el efecto ::after para las líneas decorativas bajo los títulos de sección (.section-title).

Se añade la transición y el efecto hover a las tarjetas para que se eleven ligeramente (transform: translateY(-8px)).

Se estilizan las imágenes de los ponentes para hacerlas circulares (border-radius: 50%).

Commit 5: Mejora de la accesibilidad y detalles finales.

Se añade texto alternativo (alt) a todas las imágenes para mejorar la accesibilidad.

Se ajustan los espacios y márgenes generales para una mejor legibilidad.

Se optimiza el pie de página, añadiendo un enlace al sitio web de San Valero.

Se verifica que todos los enlaces de navegación (href="#seccion") apunten correctamente a los id de las secciones.

Mayor Dificultad Encontrada y su Solución
Dificultad: El mayor desafío técnico fue probablemente la creación y personalización de la sección Hero con una imagen de fondo y una superposición oscura, asegurando al mismo tiempo que el texto permaneciera legible y que todo el conjunto fuera responsivo.

La superposición oscura se consigue típicamente con un linear-gradient, pero combinarlo correctamente con una imagen de fondo (background-image) y lograr que cubra toda la sección sin distorsionarse puede ser complejo. Además, había que asegurar que el texto (título, fecha, botón) estuviera por encima de esta capa y que el alto de la sección se adaptara bien a diferentes tamaños de pantalla.

Solución: La solución se implementó en el CSS personalizado de la siguiente manera:

Combinación de gradient e imagen: Se utilizó la propiedad background con un linear-gradient y una url() separados por comas.

css
background: linear-gradient(rgba(13,27,42,0.78), rgba(13,27,42,0.78)),
            url('San Valero Ordenadores.jpg') center/cover no-repeat;
El primer valor (linear-gradient) crea la capa de color oscuro semitransparente. El segundo valor establece la imagen de fondo, la centra (center) y la hace cubrir todo el contenedor (cover), y evita que se repita (no-repeat). El navegador apila estos fondos, quedando el gradient sobre la imagen.

Control de la altura: Se usó min-height: 70vh; en lugar de un height fijo. Esto asegura que el hero ocupe al menos el 70% de la altura de la ventana del navegador (viewport height), pero si el contenido es más grande (por ejemplo, en móviles con texto muy largo), la sección se expandirá para contenerlo sin que se recorte el texto, gracias al padding-top y padding-bottom que proporcionan el espacio interior necesario.
