# hyperblog
Curso Git-Github



Comandos utiles:

**Generales / Navegación:\n**

ls lista los archivos en la posición en el que estes

ls -al muestra todos los archivos listados y que estén ocultos

pwd -> ver en que directorio estas

cd -> cambiar de directorio

cd .. -> volver un directorio

~/proyecto1/  el signo ~ es un tipo de shortcut de nuestro home. 

mkdir -> crea una nueva carpeta

touch “nombre del archivo” -> crea un archivo .txt

Cat “nombre del archivo” -> muestra lo que tiene el archivo


**Git:**


git init

git config -> ver las configuraciones de git

git config -l -> nos ayuda ver todas las configuraciones: --

git config --global user.name “Mario aleman”

git config --global user.email “mar.alemanf@gmail.com”

git add “nombre del archivo” -> lo pone en estado de staging/espera de ser commit

git commit -m “Comentario”

git show -> muestra el ultimo commit

git log “nombre del archivo” -> muestra todos los log históricos

git diff “codigo” “codigo” -> compara entre 2 versiones del archivo

git reset borra los datos de forma permanente existen dos –hard y –soft hard elimina todo, mientras que soft solo elimina el commit pero no los archivos que tengas en el staging

git checkout --> puedes volver en el pasado sin borrar nada

git Branch --> crea una nueva ramificación

git checkout “nombre de la ramificacion” --> viaja a la nueva a ramificación.

git merge “nombre de la ramificación que queremos unir”


Git Hub


FETCH-> Traer cosas

PUSH -> Mandar cosas

Si tenemos un proyecto iniciado y queremos mandarlo a github realizamos el siguiente comando.

Git remote add origin “link/url de tu repositorio en github”.

Git fetch origin “main”

Git push origin master

git pull origin master



con el nuevo cambio de git hub es necesario realizar lo siguiente: 

Por lo tanto escribimos/o podemos configurar nuestro github para determinar rama 'main' --> a 'master'

git push origin master:main

git pull origin main –allow-unrelated-histories




Para cambiar el url

Origin es el nombre de nuestro repositorio remoto

Git remote set-url “nombre del origin” git@github.com:IPN-Mario-Aleman/hyperblog.git

Git remote -v ->para saber que link tienen



**Recomendaciones**

Antes de realizar algun commit se debe traer la última versión de nuestro repositorio.

$ alias = “git log –all –graph –decorate --oneline” -> guarda una línea de comando --> ademas de que este comando muestra de forma gráfica todos los commit realizados, asi como las ramas en ella.


git tag -a v0.1 -m "Resultado de las primeras clases del curso" 'No. del commit sin comillas' -> guarda un commit con el nombre de un tag que puede ser una nueva versión.


Crear un nuevo tag y asignarlo a un commit: git tag -a nombre-del-tag id-del-commit.

Borrar un tag en el repositorio local: git tag -d nombre-del-tag.

Listar los tags de nuestro repositorio local: git tag o git show-ref --tags.

Publicar un tag en el repositorio remoto: git push origin --tags.

Borrar un tag del repositorio remoto: git tag -d nombre-del-tag y git push origin :refs/tags/nombre-del-tag.

