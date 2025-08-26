### Comandos básicos de Git

- git init: nos permite inicializar un repositorio de forma local.

- git status: nos brinda información general de los archivos del repositorio, es decir, cuales son nuevos, cuales fueron modificados, cuales estan 'preparados' para su confirmación/guardado (commit), la rama sobre la cual estamos trabajando, entre otros datos.

- git add <nombreArchivo>: Nos permite añadir al 'Staging Area' el archivo especificado. Esta 'area' prepara los archivos que van a ser confirmados/commiteados, sino están dentro de este seguimiento no se van a tener en cuenta dentro del commit.
* Alternativa git add . -> nos permite agregar todos los elementos modificados/nuevos al staging area, sin necesidad de especificar uno por uno.

- git commit -m "comentario": Nos permite guardar/confirmar defintiivamente los cambios generados de una nueva version del proyecto. Cada uno estos commits va formado un historial de versiones, y luego si es necesario prodiamos navegar entre ellos, es decir, podes retroceder a una versión anterior. El comentario generalmente debe representar/especificar los cambios introducidos, tratar de ser lo más descriptivo posible.

- git remote add origin <url_repo_remoto>: Nos va a permitir vincular el repo local con el repositorio remoto, para poder subir los cambios a la nube, ya sea para crear de cero o actualizar futuros cambios. Este paso se suele realizar una sola vez. Esto nos va a permitir ejecutar comandos como 'push' y 'pull'.

- git push: Nos permite subir los cambios realizados desde el repo local al remoto, previamente debemos realizar al menos un commit. 

- git pull: Nos permite actualizar el repo local en base al repo remoto, es decir, traer las actualizaciones desde el repositorio remoto.


### Manejo ramas:

- git branch: nos muestra todas las ramas existentes en el repositorio. * para salir del 'bucle' shift+q.
- git branch <nombre_de_rama>: nos crear una nueva rama.
- git branch -d <nombre_rama>: Nos permite eliminar una rama.
- git branch -M <nombre_rama>: Renombrar la rama sobre la cual estamos posicionados.
- git switch <rama>: Nos permite movernos entre ramas