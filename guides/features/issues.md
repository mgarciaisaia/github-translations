# Manejando Issues
#### (Lectura de 10 minutos)

- [Introducción](#)
- [Milestones, Labels y Assignees](#milestones-labels-y-assignees)
- [Notificaciones, @mentions y referencias](#notificaciones-mentions-y-referencias)
- [Búsqueda](#b%C3%BAsqueda)
- [Información y reportes](#informaci%C3%B3n-y-reportes)
- [Otros usos para Issues](#otros-usos-para-issues)
- [Fin](#fin)

Los issues (_incidencias_) son una excelente manera de administrar tareas, mejoras o errores en tus proyectos. Son un poco como un e-mail, pero que podés compartir y discutir con el resto de tu equipo. La mayoría de los proyectos de software tienen algún tipo de bug tracker (_administrador de bugs_). El de GitHub se llama **Issues**, y tiene su propia sección en cada repositorio.

![Botón de Issues en un repositorio de GitHub](https://guides.github.com/features/issues/navigation-highlight.png)

Por ejemplo, miremos [la sección de Issues del repositorio de Bootstrap](https://github.com/twbs/bootstrap/issues):

![Sección de Issues del repositorio de Bootstrap](https://guides.github.com/features/issues/listing-screen.png)

El issue tracker de GitHub es especial por estar enfocado en la colaboración, las referencias y el excelente formateo de texto. Un issue común en GitHub se ve algo así:

![Un issue en GitHub](https://guides.github.com/features/issues/example-issue.png)

- El **título** y la **descripción** cuentan de qué trata el issue.
- Las **etiquetas** de colores ayudan a categorizar y filtrar los issues (tal como las etiquetas en los e-mails).
- El **milestone** (_hito_) funciona como un contenedor de issues. Sirve para agrupar issues sobre una tarea específica o sobre una etapa del proyecto (por ejemplo, _Sprint Semana 34_ o _Release 1.0_).
- El **assignee** (_designado_) es el responsable de trabajar en ese issue en un momento determinado.
- Los **comentarios** permiten que quienes tengan acceso al repositorio puedan opinar sobre el issue.

## Milestones, Labels y Assignees
Al acumular varios issues, se complica encontrar los que te interesan. Los **milestones**, **labels** y **assignees** te permiten filtrar y categorizar los issues.

Podés cambiar o agregar los milestones, assignees o labels clickeando en sus respectivos íconos de engranaje en la barra lateral de la derecha.

![Milestones, labels y assignees](https://guides.github.com/features/issues/labels.png)

Si no ves los botones de engranajes significa que no tenés permisos para editar el issue. Podés pedirle al owner (_dueño_) del repositorio que te agregue como colaborador para obtener acceso.

### Milestones

![Milestones](https://guides.github.com/features/issues/milestones.png)

Los milestones son grupos de issues que corresponden al mismo proyecto, tarea o período de tiempo. Se los suele usar de maneras muy diversas en los proyectos de software. Algunos ejemplos de milestones en GitHub incluyen:

- **Beta Launch** - bugs que necesitan ser resueltos antes de poder publicar una versión beta de tu proyecto. Es una buena forma de no olvidarte de nada.
- **Sprint de Octubre** - marcá todas las tareas en las que quieras trabajar durante octubre. Útil para enfocarse cuando hay demasiadas cosas para hacer.
- **Rediseño** - issues relacionados al rediseño de tu proyecto. Ayuda a juntar ideas sobre qué vas a tener que hacer.

### Labels

Las labels son geniales para organizar distintos tipos de issues. Cada issue puede tener tantas labels como gustes, y podés filtrarlos por una o más labels al mismo tiempo.

![Labels](https://guides.github.com/features/issues/labels-listing.png)

### Assignees

Cada issue puede tener un assignee - la persona responsable de avanzar con ese issue. Los assignees se seleccionan del mismo modo que los milestones: desde el ícono del engranaje.

## Notificaciones, @mentions y referencias

Usando @mentions (_"at mentions"_, _menciones_) y referencias en tus issues, podés notificar a otros usuarios y equipos de GitHub, y conectar los issues entre sí. Proveen una forma flexible de involucrar efectivaemnte a la gente correcta para resolver los issues, y son fáciles de aprender y usar. Funcionan en todos los campos de texto en GitHub - son parte de la sintaxis de formateo de texto llamado [GitHub Flavored Markdown](https://help.github.com/articles/writing-on-github#name-and-team-mentions-autocomplete).

![Escribiendo GitHub Flavored Markdown en un Issue](https://guides.github.com/features/issues/markdown-example.png)

Si querés aprender más, podés leer [Mastering Markdown](http://guides.github.com/features/mastering-markdown/).

### Notificaciones

Las [notificaciones](https://github.com/notifications) son la forma de mantenerte al día con tus issues en GitHub. Podés usarlas para ver las novedades en los issues de un repositorio, o sólo para enterarte cuando alguien te necesita para avanzar un issue.

Hay dos formas de recibir notificaciones: por e-mail, y por la web. Podés configurar cómo recibir tus notificaciones [en tus preferencias](https://github.com/settings/notifications). Si esperás recibir muchas notificaciones, te recomendamos recibir notificaciones en la web + e-mail para **Participating** (issues en que participás), y sólo web para **Watching** (issues que estás siguiendo).

![Configurando notificaciones](https://guides.github.com/features/issues/notifications.png)

Con estas preferencias, recibís e-mails cuando la gente te menciona directamente, y podés entrar en la web para ponerte al día con los repositorios que te interesan.

Podés acceder a tus notificaciones a través de la [página de notificaciones](https://github.com/notifications). Esta página está pensada para ojear varias notifiaciones a la vez y marcarlas como leídas o silenciarlas. Probá de usar los atajos de teclado para acelerar tu trabajo acá - apretá `?` estando en la página para ver qué atajos tenés disponibles.

![Notificaciones](https://guides.github.com/features/issues/notification.png)

Los threads silenciados (_muted_) no van a volver a aparecerte mientras nadie te @mencione directamente. Es una buena estrategia para los threads en los que no estás muy interesado (quizá un sub-sistema del proyecto en el que no tenés mucho que ver). Si marcás un issue como leído, se va a mantener así hasta que alguien comente nuevamente en él.

GitHub también sincroniza el estado de leído/no leído a través de las notificaciones por e-mail - si leés una notificación en tu cliente de mail, va a marcarse como leído en la interfaz web (asegurate de habilitar las imágenes en tu cliente de mail para poder usar esta funcionalidad).

### @mentions

Las @mentions son la forma de referenciar a otros usuarios de GitHub dentro de los issues. Tanto en la descripción del issue como en cualquier comentario, escribí @nombredeusuario de otro usuario de GitHub para mandarle una notificación. Funciona bastante similar a como Twitter usa las @mentions.

Se suele usar la sintaxis `/cc` (abreviación de _"carbon copy"_, _copia en carbónico_) para incluir gente en los issues:

> Parece que el nuevo widget de formulario está roto en Safari. Cuando lo pruebo y creo el widget, Safari crashea. Puedo reproducirlo en 10.8, pero no en 10.9. ¿Será un bug del browser?
>
> /cc @kneath @jresig

Esto está bueno para cuando sabés a qué usuarios específicos incluir, pero a veces estás trabajando entre equipos y no sabés muy bien quién va a poder ayudarte. Las @mentions también funcionan para los equipos en tu organización de GitHub. Si creás un equipo llamado _browser-bugs_ en la organización @acmeinc, podés referenciar al equipo usando una @mention:

> /cc @acmeinc/browser-bugs

Esto va a enviarle notificaciones a cada miembro de ese equipo.

### Referencias

A menudo los issues dependen de otros issues, o al menos se relacionan de algún modo, y querés establecer alguna conexión entre ambos. Podés referenciar issues tipeando un numeral (`#`) seguido del número de issue.

> Hey, @kneath, creo que el problema comenzó en #42

Cuando hagas esto, se va a crear un evento en el issue #42 que se ve algo así:

![Referencias en issues](https://guides.github.com/features/issues/reference.png)

¿Y para issues de otros repositorios? Simplemente incluí antes el nombre del repo, como en `kneath/example-project#42`.

Uno de los usos más interesantes de GitHub Issues es poder referenciar issues directamente desde los commits. Incluí el número de issue dentro del mensaje de un commit.

![Referenciando issues desde un commit](https://guides.github.com/features/issues/commit.png)

Prefijando tus commits con "Fixes", "Fixed" o "Fix" (_"arregla"_), "Closes", "Closed" o "Close" (_"cierra"_) vas a cerrar automáticamente el issue al mergear ese commit a master.

Las referencias permiten conectar el trabajo hecho con el bug que está tratando de resolver, y son geniales para dar más visibilidad a la historia de tu proyecto.

## Búsqueda

En la parte superior de cada página hay una caja de búsqueda que te permite buscar en los issues.

![Buscando Issues](https://guides.github.com/features/issues/search.png)

Podés acotar las búsquedas por:

- Términos de búsqueda, como, por ejemplo, [todos los issues que mencionan la sidebar](https://github.com/twbs/bootstrap/issues?q=sidebar) (barra lateral)
- Estado, como ser [todos los issues _cerrados_ que mencionan la sidebar](https://github.com/twbs/bootstrap/issues?q=sidebar+is%3Aclosed)
- Assignee, como [todos los issues _asignados a @mdo_ que mencionan la sidebar](https://github.com/twbs/bootstrap/issues?q=sidebar+is%3Aclosed+assignee%3Amdo)

El [artículo de ayuda sobre búsqueda de issues](https://help.github.com/articles/using-search-to-filter-issues-and-pull-requests) muestra otras formas de buscara: usando las fechas de creación/actualización, labels, autores, cantidad de comentarios, dueño del repositorio y más.

## Información y reportes

Fuera de la sección de issues hay dos otras páginas que te ayudan a resumir qué está pasando con los issues de un repositorio, y de todos tus repositorios en general.

### El dashboard de issues

Si estás buscando un listado más amplio de todos tus issues en distintos proyectos, el [dashboard de issues](https://github.com/issues) puede serte muy útil. El dashboard funciona parecido a la sección de issues, pero los agrupa de diferentes maneras:

- Todos los issues de los repositorios tuyos y en los que sos colaborador
- Los issues asignados a varios
- Los issues que creaste

Si usás organizaciones, cada una tiene su propio dashboard que sólo muestra los issues de esa organización.

### Pulse

Abajo de todo, cada repositorio tiene una sección llamada **Pulse** (_pulso_) - un resumen de todo lo que pasó en ese repositorio la última semana (o el último día, o los últimos 3 meses, etc).

![Pulse](https://guides.github.com/features/issues/pulse.png)

Es bastante útil para ponerte al día con repositorios que tuviste abandonados durante algún tiempo y que no querés la granularidad de leer cada notificación.

## Otros usos para Issues

Los issues son útiles para hacer seguimiento de todo tipo de cosas, y GitHub es un gran lugar para colaborar y compartir fácilmente tus issues. Acá hay algunos de nuestros favoritos:

- [Seguidor de problemas para tu casa](https://github.com/frabcus/house/issues?labels=building&state=open), incluyendo perlitas como que [**la puerta está colocada del lado incorrecto**](https://github.com/frabcus/house/issues/58)
- [Seguidor de problemas para tus proyectos open source](https://github.com/joyent/node/issues)
- [Pedidos de recetas](https://github.com/newmerator/recipes/issues) (¿tendrás una buena [receta de pizza libre de glúten](https://github.com/newmerator/recipes/issues/3)?)

## Fin

**Felicitaciones**, ¡fue bastante para leer! La administración de issues es una de las herramientas más poderosas que tienen los desarrolladores. Supongo que todo lo que queda ahora es ponerse a _efectivamente_ resolver esos issues.
