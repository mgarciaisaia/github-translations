# Armando tu proyecto en GitHub
#### (Lectura de 5 minutos)

El software está en el corazón de GitHub, y el código es el ADN del software. Si te estás registrando, es muy probable que tengas algo de código que quieras pushear a GitHub. ¡Y esa es una idea fantástica!

Estas son algunas buenas razones para pushear proyectos a GitHub:

- **Versionado** - Todo lo que hay en GitHub está almacenado en [Git](http://git-scm.com/), el mejor sistema de control de versiones que hay dando vueltas. Versionar te permite experimentar y cometer errores en tu código sin arruinar tu producto final.

- **Mantener tu código en un lugar** - Ya sea que trabajes en varias computadoras o simplemente quieras sacar algunos proyectos de tu computadora, GitHub es el lugar perfecto para almacenar tus proyectos online.

- **Colaboración** - Una vez que tu código está en GitHub, podés invitar a otros a trabajar en tu código con vos. Con enviarles un enlace te van a poder ayudar a debuggear un problema.

![Vista del repositorio mbostock/d3](http://guides.github.com/overviews/desktop/repository.png)

Una vez que tu proyecto está en GitHub, te damos una URL para cada archivo de tu proyecto. Por ejemplo, este es el popular proyecto [d3](https://github.com/mbostock/d3) de Mike Bostock para crear documentos orientados a datos con Javascript.

Usamos bastante las palabras Git y GitHub en este artículo, así que mejor aclaremos qué significan:

- **Git** - La herramienta de versionado sobre la que se basa GitHub.

- **GitHub** - Nuestra empresa y el nombre de nuestro producto. Construimos software y sitios que te ayudan a interactuar con repositorios Git agradablemente.

- **GitHub.com** - El sitio en el que entrás para ver tus repositorios online.

- **GitHub Desktop** - Una aplicación que podés instalar en tu computadora para ayudarte a sincronizar tu código local con GitHub.com

## GitHub Desktop
GitHub Desktop es la manera más fácil de subir código a GitHub.com. No vas a necesitar aprender instrucciones de línea de comando, claves de SSH o terminología compleja de Git. Todo lo que necesitás es tu Mac o PC con Windows y [una cuenta de GitHub.com](https://github.com/join).

Podés descargar GitHub Desktop para [**Mac**](http://mac.github.com/) y [**Windows**](http://windows.github.com/). Una vez que instalás GitHub Desktop, un pequeño wizard inicial te guiará a través de algunas configuraciones básicas, y te ayudará a conectar GitHub Desktop con tu cuenta de GitHub.com.

### Iniciar tu proyecto en GitHub Desktop

La manera más simple de incluir tu proyecto en GitHub Desktop es arrastrando la carpeta con tu código a la pantalla principal de la aplicación.

_Nota: los ejemplos muestran la aplicación para Mac, pero el flujo es el mismo para la aplicación de Windows._

![Arrastrando una carpeta a la aplicación para Mac](http://guides.github.com/overviews/desktop/mac-dragndrop.jpg)

Si usás un repostiorio Git existente, podés saltearte hasta la sección de pushear tu código a GitHub.com.

Si la carpeta no es un repositorio Git, GitHub Desktop te va a ofrecer convertirla en un repositorio. Convertir tu proyecto en un repositorio Git no va a eliminar ni arruinar los archivos que ahí estén - simplemente va a crear algunos archivos ocultos que permiten a Git hacer su magia.

![Inicializando un repositorio en la aplicación para Mac](http://guides.github.com/overviews/desktop/mac-gitinit.jpg)

### Tu primer commit

Los repositorios Git se basan en _commits_ - versiones de tu código en un punto determinado en el tiempo. Necesitás hacer al menos un commit para poder pushear tu código a GitHub.com.

![Commiteando en la aplicación para Mac](http://guides.github.com/overviews/desktop/mac-commit.jpg)

Navegá a la pestaña **Changes** ("Cambios") y clickeá **Commit** para crear tu primer commit. Tenés que crear un nuevo commit cada vez que cambiás tus archivos. Crear un commit es como grabar un archivo - le estás diciendo a Git que querés que recuerde ese momento en la historia.

Creá tantos commits como quieras localmente. Nadie más que vos va a poder verlos hasta que no los pushees a GitHub.com.

## Pushear tu código a GitHub.com

![Pusheando en la aplicación para Mac](http://guides.github.com/overviews/desktop/mac-push.jpg)

Clickeá el botón "Push to GitHub" ("Pushear a GitHub") que está en la esquina superior derecha y GitHub Desktop te va a preguntar qué tipo de repositorio crear:

- **Repositorio público** - Cualquiera puede ver un repositorio público, pero vos elegís quiénes pueden commitear (hacer cambios) a él. Podés crear tantos repositorios públicos como quieras en GitHub.com gratuitamente.

- **Repositorio privado** - Por defecto, sólo vos podés ver un repositorio privado. Vos elegís quiénes pueden ver y commitear a este repositorio agregando colaboradores. Los repositorios privados requieren [una suscripción paga](https://github.com/settings/billing) a GitHub.com.

Ahora que publicaste el repositorio, lo tenés en dos lugares:

- **Repositorio local en tu computadora** - Podés trabajar en este repositorio sin estar conectado a Internet usando GitHub Desktop. Acá es donde editas archivos y hacés cambios a tu proyecto.

- **Repositorio remoto en GitHub.com** - Podés enviarle links a tu repositorio en GitHub.com a otras personas para que puedan ver tu código y usar todas las otras características de GitHub (como la administración de Issues y los Pull Requests).

Cada vez que hagas cambios a tu repositorio local vas a necesitar sincronizar tus cambios (clickeando el botón en la esquina superior derecha de GitHub Desktop) para asegurarte de que estén online.


## Obteniendo código de GitHub.com

Si querés obtener código desde GitHub.com a tu computadora o sincronizar cambios entre muchas computadoras, vas a necesitar pullear cambios o clonar un repositorio:

- **Pullear cambios** - Clickeá el botón de "Sync" arriba a la derecha en GitHub Desktop para traer código desde un repositorio online (por ejemplo, cambios que un colega haya pusheado) hacia tu computadora. _Nota: esto también va a pushear cambios que no hayas pusheado aún._

- **Clonar un repositorio** - Clickeá el botón "Clone in Desktop" ("Clonar en Desktop") en GitHub.com para crear una nueva copia de un repositorio en tu computadora.


## ¡Celebrá!

¡Ahora sabés la instalación básica de un proyecto en GitHub!

* Descargá y usá GitHub Desktop.
* Commiteá cada vez que alcanzás una meta o querés guardar tu progreso.
* Sincronizá tus cambios con GitHub.com para pushear tus nuevos commits y pullear commits de otros.

¡Y ya está! Acá hay un puñado de [cosas geniales que podés hacer con los repositorios](https://github.com/features).