#Hola, mundo
#### (Lectura de 10 minutos)

- [Introducción](#)
- [Crear un repositorio](#crear-un-repositorio)
- [Abrir un issue](#abrir-un-issue)
- [Crear un branch](#crear-un-branch)
- [Hacer un _commit_](#hacer-un-commit)
- [Abrir un Pull Request](#abrir-un-pull-request)
- [_Mergear_ un Pull Request](#mergear-un-pull-request)

El proyecto **Hola, mundo** es una tradición legendaria en el mundo de la programación. Es un ejercicio simple que te permite arrancar cuando estás aprendiendo algo nuevo. ¡Arranquemos con GitHub!

GitHub es una plataforma para alojar proyectos y colaborar en ellos. No tenés que preocuparte por perder los datos en tu disco rígido o administrar proyectos entre distintas computadoras - mantenete sincronizado desde todos lados. Más importante, GitHub es un flujo de trabajo colaborativo y asincrónico para construir software mejor, en conjunto.

Esta guía te llevará por los Escenciales de GitHub: **Repositorios**, **Ramas** (_branches_), **Commits**, **Issues* y **Pull Requests**.

Con estos conocimientos, vas a llegar bastante lejos. Y con este repositorio `hello-world` vas a tener un lugar en que almacenar ideas (futuros repositorios, como [jlord/hello-world](https://github.com/jlord/hello-world)), recursos u otras notas generales, incluso para discutir con otros (como [hollman/feedback](https://github.com/holman/feedback)).

### Zona libre de instalación y código

Vamos a completar todas las tareas de este tutorial usando GitHub.com, así que no necesitás conocer la línea de comandos ni instalar Git (que es el software de versionado de cambios sobre el que se basa GitHub). Ni siquiera necesitás saber cómo escribir código. Sin embargo, vas a necesitar una cuenta de GitHub, así que ¡registrate si no tenés una!

> **Tip:** abrí esta guía en una ventana (o pestaña) aparte del navegador para que puedas leerla mientras seguís los pasos del tutorial.

## Crear un repositorio

Un **repositorio** es la unidad básica de GitHub, más comunmente un único proyecto. Los repositorios pueden contener directorios y archivos, incluídas imágenes - lo que sea que tu proyecto necesite. Dado que recomendamos incluir un README - _"leeme"_ - (o un archivo que describa el proyecto) en cada repositorio, GitHub simplifica agregar uno al momento de crear tu nuevo repositorio. _También ofrece otras opciones comunes como un archivo de licencia, pero podemos saltearnos eso por ahora._

### Para crear un nuevo repositorio

1. Clickeá el ícono del + al lado de tu nombre de usuario, arriba a la derecha.
2. Llamá `hello-world` a tu repositorio.
3. Escribí una descripción corta.
4. Elegí **Initialize this repository with a README** (_inicializar este repositorio con un README_).

![new-repo-form](https://guides.github.com/activities/hello-world/create-new-repo.png)

Clickeá **Create repository** (_crear repositorio_). ¡Boom, repositorio! :boom:

## Abrir un issue

Un **issue** (_incidencia_) es una nota en un repositorio sobre algo que necesita atención. En GitHub podés etiquetar, buscar y asignar issues, facilitando la administración de un proyecto activo.

Ya tenés un repositorio ahora, pero está bastante vacío. Podría incluir un README con más información para que la gente sepa de qué se trata. ¡Abrí un issue!

### Abrir un issue para editar el README

1. Clickeá la pestaña de Issues en la barra lateral.
2. Clickeá **New issue** (_Nuevo issue_).
3. Dale un título y descripción a tu issue.

![issue](https://guides.github.com/activities/hello-world/issue.png)

Clickeá **Submit new Issue** (_enviar nuevo issue_) cuando hayas terminado. Ahora ese issue tiene una ubicación permanente (una URL) que podés referenciar incluso después de cerrado.

Lo próximo es trabajar para editar tu README y cerrar este issue.

## Crear un Branch

**Branchear** es la forma de trabajar en diferentes partes de un repositorio al mismo tiempo.

Cuando creás un repositorio, por defecto tiene un branch llamado `master`. Podés seguir trabajando en esa branch y tener esa sola, y está bien. Pero si tenés otra característica o idea en la que trabajar, podés crear otra branch, partiendo de `master`, así podés dejar `master` en ese estado de trabajo.

Cuando creás un branch, estás haciendo una copia del branch original como estaba en ese momento en la historia (como una foto instantánea). Si el branch original cambia cuando estás trabajando en tu nuevo branch, no hay drama, siempre podés traerte esas actualizaciones.

![Una branch](https://guides.github.com/activities/hello-world/branching.png)

Podés tener, en algún momento de tu vida, distintas versiones guardadas de un archivo, como "historia.txt", "historia-jose-editada.txt", "historia-susana-editada.txt". Los branchs logran los mismos objetivos, pero son más simples de manejar en los repositorios de GitHub.

En GitHub, nuestros desarrolladores, escritores y diseñadores usan branchs para mantener separadas las correcciones de bugs y las nuevas características de nuestro branch `master`, el de producción. Cuando una característica o corrección está lista, el branch se mergea (_integra_) a `master`.

### Para crear un nuevo branch

1. Andá a tu nuevo repositorio `hello-world`.
2. Clickeá el menú desplegable que está arriba de la lista de archivos que dice **branch: master**.
3. Tipeá el nombre del branch, `readme-edits`, en la caja de texto de nuevo branch.
4. Seleccioná la opción azul **Create branch** (_crear branch_) o apretá "Enter" en tu teclado.

![branch gif](https://guides.github.com/activities/hello-world/readme-edits.gif)

Ahora tenés dos branchs, `master` y `readme-edits`. Se ven exactamente igual, pero ¡no por mucho! Ahora vamos a agregar nuestros cambios en el nuevo branch.

## Hacer un _commit_

En GitHub, los cambios guardados se llaman **commits*. Los commits son bastante gloriosos, porque un conjunto de ellos representan la historia de tu proyecto.

Cada commit tiene un **mensaje de commit** asociado, que es una descripción explicando por qué se hizo un cambio en particular. Gracias a esos mensajes, vos y otros pueden leer la historia de commits y entender qué cosas hiciste y por qué.

Aún deberías estar en la vista de código de tu branch `readme-edits`, ¡hagamos algunos cambios!

### Para commitear cambios

1. Clickeá el archivo README.
2. Clickeá *Edit* (_editar_).
3. En el editor, escribí algún texto, contá algo de vos.
4. Escribí un mensaje de commit que describa tus cambios.

![commit](https://guides.github.com/activities/hello-world/edit-top.png)
![commit](https://guides.github.com/activities/hello-world/edit-bottom.png)

Clickeá **Commit changes** (_commitear cambios_). Ahora esos cambios se aplicaron sobre tu archivo README en tu branch `readme-edits` y ese branch tiene contenido y commits distinto al de `master` (¡tal como debería!).

## Abrir un Pull Request

Los Pull Requests son el corazón de la colaboración en GitHub. Cuando hacés un **pull request** estás proponiendo tus cambios y pidiéndole a alguien que incluya tu contribución - es decir, mergearlos en su branch. Los Pull Requests de GitHub te permiten comparar el contenido de dos branchs. Los cambios, adiciones y substracciones, se muestran en verde y rojo, y son llamados **diffs* (_diferencias_).

Ni bien empieces a hacer un cambio, podés abrir un pull request. La gente usa los pull requests para discutir sobre los commits (revisión de código) incluso antes de que el código esté finalizado. De este modo podés obtener feedback mientras estás desarrollando, o ayuda cuando te trabás en algo.

Usando el [sistema de @menciones](https://github.com/blog/821-mention-somebody-they-re-notified) de GitHub en tu mensaje del pull request podés pedir feedback a personas o equipos específicos, estén del otro lado del pasillo o a diez usos horarios de distancia.

Incluso podés abrir, como estamos haciendo acá, un pull request en tu propio repositorio y mergearlo vos mismo. Es una buena forma de aprender el proceso antes de trabajar en proyectos más grandes.

### Crear un Pull Request para los cambios del README

_Clickeá en la imagen para verla más grande_

| **Paso** | **Gráfico** |
|----------|-------------|
| Clickeá el ícono de Pull Request en la barra lateral, después en la página de Pull Requests clickeá el botón verde de **Create pull request** (_Crear pull request_). | [![create pr](https://cloud.githubusercontent.com/assets/1305617/2543808/73059f0a-b5f7-11e3-928e-745e9f9a5c75.gif)](https://cloud.githubusercontent.com/assets/1305617/2543808/73059f0a-b5f7-11e3-928e-745e9f9a5c75.gif) |
| Seleccioná el branch que creaste, `readme-edits`, para compararlo con `master` (el original)| [![branch](https://guides.github.com/activities/hello-world/pick-branch.png)](https://guides.github.com/activities/hello-world/pick-branch.png) |
| Revisá tus cambios en los diffs en la página Compare (_compará_), y asegurate de que es lo que querés enviar. | ![diff](https://guides.github.com/activities/hello-world/diff.png) |
| Cuando estés seguro de que son los cambios que querés enviar, clickeá el gran botón verde de **Create Pull Request** (_crear pull request_). | [![create-pull](https://guides.github.com/activities/hello-world/create-pr.png)](https://guides.github.com/activities/hello-world/create-pr.png) |
| Dale un título a tu pull request y, dado que se relaciona directamente con un issue abierto, incluí "Fixes #" (_"corrije"_) y el número de issue en el título. Escribí una breve descripción de tus cambios. _Es importante que el mensaje esté en inglés para que GitHub lo reconozca._ | [![pr-form](https://guides.github.com/activities/hello-world/pr-form.png)](https://guides.github.com/activities/hello-world/pr-form.png) |

Cuando hayas terminado con tu mensaje, ¡clickeá **Send Pull Request** (_enviar pull request_)!

> **Tip:** Podés usar [emoji](https://github.com/blog/1289-emoji-autocomplete) y [arrastrar imágenes y gifs](https://github.com/blog/1347-issue-attachments) en los comentarios y pull requests.

## _Mergear_ tu pull request

Es hora de unificar tus cambios - _integrar_ tu branch `readme-edits` al branch `master`.

1. Clickeá el botón verde para mergear los cambios a `master`.
2. Clickeá **Confirm merge** (_Confirmar merge_).
3. Animate y eliminá este branch, dado que sus cambios ya fueron integrados, con el botón de **Delete branch** (_eliminar branch_) en la caja violeta.

![merge](https://guides.github.com/activities/hello-world/merge-button.png)
![delete](https://guides.github.com/activities/hello-world/delete-button.png)

Si volvés a ver el issue que habías abierto, ¡ahora está cerrado! Como incluiste "fixes \#1" en el título de tu pull request, ¡GitHub se encargó de cerrar ese issue cuando se mergeó el pull request!

## ¡Celebrá!

¡Aprendiste a hacer un pull request en GitHub! :tada: :octocat: :zap:

Para que puedas alardear, esto es lo que lograste en este tutorial: creaste un repositorio, branch, issue y pull request, y después ¡mergeaste un pull request! ¡Ya podés mostrar tus [cuadraditos de contribuciones](https://help.github.com/articles/viewing-contributions)!
Si querés aprender más sobre el poder de los pull requests, te recomendamos leer la [Guía del GitHub Flow](https://guides.github.com/introduction/flow/index.html). También podés visitar [GitHub Explore](http://github.com/explore) e involucrarte en algunos proyectos de código abierto  :octocat:

> **Tip**: revisá nuestras otras [Guías](http://guides.github.com/) (acá [en Español](https://github.com/mgarciaisaia/github-translations/tree/spanish/guides)) y el [Canal YouTube](http://youtube.com/githubguides) para más tutoriales sobre GitHub.
