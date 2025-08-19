### Comandos básicos de Git

git init: nos permite inicializar un repositorio de forma local.

git status: nos brinda información general de los archivos del repositorio, es decir, cuales son nuevos, cuales fueron modificados, cuales estan 'preparados' para su confirmación/guardado (commit), la rama sobre la cual estamos trabajando, entre otros datos.

git add <nombreArchivo>: Nos permite añadir al 'Staging Area' el archivo especificado. Esta 'area' prepara los archivos que van a ser confirmados/commiteados, sino están dentro de este seguimiento no se van a tener en cuenta dentro del commit.
* Alternativa git add . -> nos permite agregar todos los elementos modificados/nuevos al staging area, sin necesidad de especificar uno por uno.

git commit -M "comentario": Nos permite guardar/confirmar defintiivamente los cambios generados de una nueva version del proyecto. Cada uno estos commits va formado un historial de versiones, y luego si es necesario prodiamos navegar entre ellos, es decir, podes retroceder a una versión anterior. El comentario generalmente debe representar/especificar los cambios introducidos, tratar de ser lo más descriptivo posible.