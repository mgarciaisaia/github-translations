# Duplicando un repositorio

Para crear un duplicado de un repositorio sin forkearlo, necesitás correr un comando `clone` especial contra el repositorio original, y hacer un push-copia a uno nuevo. Esto funciona con cualquier repositorio git, no sólo los hosteados en GitHub.

En los próximos ejemplos, el repositorio al que intentás pushear (como ser `usuario/nuevo-repositorio` o `usuario/duplicado`) deberían estar ya creados en GitHub. Visita la guía [Creando un nuevo repositorio](https://help.github.com/articles/creating-a-new-repository) para más información.


## ¡Hagámoslo!

Para hacer un duplicado exacto, necesitás hacer primero un clon bare y un push mirror:

```
$ git clone --bare https://github.com/usuario/repositorio-original.git
# Crear un clon bare del repositorio

$ cd repositorio-original.git
$ git push --mirror https://github.com/usuario/repositorio-nuevo.git
# Mirror-push al nuevo repositorio

$ cd ..
$ rm -rf repositorio-original.git
# Borramos nuestro repositorio local temporal
```

Si querés espejar un repositorio que está en otra ubicación, e ir actualizándolo junto con el original, podés hacer un clon mirror y pushear los cambios periódicamente.

```
$ git clone --mirror https://github.com/otro-usuario/repositorio-a-espejar.git
# Hacer un clon bare mirroreado del repositorio

$ cd repositorio-a-espejar.git
$ git remote set-url --push origin https://github.com/usuario/espejado
# Establecer la ubicacion del mirror
```

Así como un clon bare, un clon espejado incluye todos los branches y ramas remotos, pero todas las referencias locales serán sobreescritas cada vez que hacés `fetch`, por lo que siempre será igual al repositorio original. Establecer la URL para el push simplifica el pushear a tu mirror. Para actualizar tu mirror, fetcheá los cambios y pusheá, lo que puede ser automatizado corriendo un cron-job.

```
$ git fetch -p origin
$ git push --mirror
```
