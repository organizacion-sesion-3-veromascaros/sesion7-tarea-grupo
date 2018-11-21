# sesion7-tarea-grupo

Requisitos 

El ejercicio que se propone consiste en construir con HTML5 y CSS3 (sin JavaScript) una galería de seis o más imágenes,inicialmente dispuestas en círculo como miniaturas y sensibles al ratón de forma que en cada momento se pueda elegir una que entonces, mediante una transición gradual, pase a mostrarse de forma destacada (al menos en tamaño) y con su orientación natural en el centro exacto del círculo. El posicionamiento de las miniaturas sobre el perímetro del círculo ha de ser preciso, sus centros deben quedar equiespaciados y la rotación de cada una de ellas debe hacer que la mediatriz de su base pase por el centro del círculo.

La forma principal de elegir imágenes será haciendo clic con el ratón. Como este comportamiento se consigue haciendo uso de la pseudoclase :focus y requiere dotar de atributos tabindex a los elementos que alberguen las imágenes de la galería, se debe dotar al conjunto de un orden de tabulación razonable que recorra todas las imágenes en sentido horario a partir de las doce (o bien prohibir, con tabindex=-1, el acceso a las imágenes mediante tabulador).

Además, la galería debe formar parte de un contenedor y quedar centrada en él, tras un título y un párrafo explicativo que deben quedar visualmente fuera de ese contenedor por estar también fuera en la estructura HTML de la página.

Y se exige que el código HTML de la página sea declarado válido por html5.validator.nu (o se habrá de justificar que los errores detectados no son tales).

Detalles técnicos adicionales
Algunos detalles técnicos que se pueden valorar positivamente son los siguientes:
- Independencia de la hoja de estilo, ubicada en fichero aparte.
- Codificación reutilizable que, aparte de conseguir que cada una de las imágenes se muestre siempre centrada, horizontal y verticalmente, dentro de un elemento cuadrado o rectangular propio de un tamaño igual para todas, haga trivial sustituir las imágenes de la galería por otras (posiblemente con otros tamaños y otras proporciones originales) sin perder ese centrado. Obviamente, también hay que conseguir que la forma en la que se muestre cada imagen respete siempre sus proporciones originales.
- Transiciones más complejas que las del ejemplo (donde todas las propiedades se modifican al mismo ritmo lineal), siempre que el efecto conseguido con ello sea razonable.
- Empleo razonable de otras propiedades CSS como bordes, colores, sombras...

Sin embargo, y para evitar perder el tiempo replicando para diferentes navegadores declaraciones CSS que afecten a propiedades experimentales, no se valorará el hecho de preparar la galería para funcionar en varios navegadores. Se debe elegir uno entre Chrome, Firefox y Opera y especificar con cuál (indicando también la correspondiente versión) se ha comprobado el correcto funcionamiento de la galería.
Por otra parte, se valorará negativamente cualquier empleo inadecuado de elementos HTML o propiedades CSS y, en particular:
- La utilización de HTML para controlar aspectos visuales que deberían especificarse en la hoja de estilo.
- La omisión de <!doctype html> o elementos estructurales importantes como html, head, title, body, header o h1.
- El empleo de reglas CSS con selectores redundantes como en el par div.container, div.container:hover.

