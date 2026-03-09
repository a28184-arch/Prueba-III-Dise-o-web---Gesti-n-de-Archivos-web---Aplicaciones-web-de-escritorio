# Jornada Tecnológica San Valero 2026
Descripción del proyecto
Página web pa la jornada tecnológica del Centro San Valero que se celebra el 12 de marzo de 2026. Está hecha con Bootstrap 5 pa que quede chula y se vea bien en móviles y ordenadores. Tiene toa la info del evento: programa, ponentes y formulario pa apuntarse.

Secciones y columnas de Bootstrap
Sección	Columnas usadas	Distribución
Cabecera	col-6 + col-6	Logo a la izquierda y menú a la derecha
Hero principal	col-12	Título y botón a lo ancho
Programa	col-md-4 (x3) + col-md-6 (x2)	3 columnas arriba, 2 abajo centradas
Ponentes	col-md-3 (x4)	4 columnas con las fotos redondas
Formulario	col-lg-6	Formulario centrado a medio lao
Componentes de Bootstrap usados
Container fluid - Pa fondos que ocupan to el ancho

Grid system - To el maquetao con filas y columnas

Botones - btn-primary y btn-lg pa el de inscripción

Formulario - Inputs, select y textarea con clases de Bootstrap

Imágenes redondas - rounded-circle pa los ponentes

Cards improvisás - Con bordes border y fondo bg-light

Sombra - shadow en el formulario

Tipografía - Clases display-3, lead, fw-bold, text-muted

Commits y mejoras
Commit 1: Estructura base

Maquetación con columnas de Bootstrap

Header con menú de navegación

Commit 2: Hero chulo

Fondo con imagen y capa oscura con gradient

Texto centrado y botón llamativo

Commit 3: Sección programa

Horarios con tarjetas en grid

Distribución 3+2 columnas

Commit 4: Ponentes con fotos

Imágenes redondas de Unsplash

Fondo azul con bg-primary

Commit 5: Formulario y footer

Inscripción con to los campos

Pie de página con dirección y copyright

La mayor dificultad
El problema: El fondo del hero principal no se veía bien porque la etiqueta de cierre </section> estaba mal colocada y la propiedad style del div estaba partida con un > mal puesto, lo que petaba too el CSS del fondo. Además la imagen no se ajustaba bien en móviles.

Cómo lo solucioné: Cerré bien too el HTML, arreglé la propiedad style que tenía una coma mal puesta y metí background-position: center; background-size: cover; background-repeat: no-repeat pa que la imagen se adapte como Dios manda en too tipo de pantallas.
