Resumen de GIT

https://try.github.io/

Documentación de Git en Español:
https://git-scm.com/book/es/v1/Empezando

Dudas:
Existe algún editor de texto como vim o nano integrado en el powershell(cmd)?

Iniciar Repositorio:
git init

Clonar Repositorio:
git clone <url_del_repositorio>

Estado de los Archivos:
Saber que archivos se han modificado.
git status

Configurar Git:
git config --global user.name "Cristian Flores"
git config --global user.email "cristian.flores@gmail.com"
git config --global core.editor atom/ .. (el editor debe estar configurado en las variables de entorno)
mas acciones:
git config --list

Ver cambios.
Se puede ver el cambio de un archivo en especifico.
git diff


Git almacena el repositorio de manera oculta (el nombre de la carpeta es .git).

Pasos para hacer seguimiento:
Guardo el archivo
Lo añado al área de preparación[]
Le indico a git que archivos pondre en el commit
git add <nombre_archivo>

La operación contraria a git add <nombre_archivo> es 
git reset <nombre>

Hago un commit: guardo una versión en el repositorio local[]
Es como hacer un checkpoint o salvar.
El mensaje del commit debe ser una descripción de los cambios.
git commit -m "mensaje del commit"

Eliminar un archivo del repositorio:
git rm <nombre_archivo>

Issues: 
Para reportar problemas.
Para gestionar tareas dentro del equipo.

Ya entre al brach...??