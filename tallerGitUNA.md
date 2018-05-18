```
https://jiffyclub.github.io/2015-07-06-scipy/slides-local_version_control.html#/5
http://slides.com/abostroem/collaborating_using_git#/
http://slides.com/abostroem/deck-4#/
```
# ¿Qué es [Git](https://git-scm.com/)?
* Es un sistema de **control de versiones**
* Creado por Linus Torvalds durante la creación de Linux
* Software libre

# ¿Para qué?
* Trabajos colaborativos o que deben de ser revisados muchas veces
    + Tesis
    + Artículos
    + Proyectos finales de cursos
* Respaldar archivos importantes

# ¿Cómo usarlo?
* [Instalar](https://git-scm.com/downloads) Git
* Abrir linea de comandos
    + También se puede acceder desde otros programas como RStudio, etc.
* Ir al directorio de trabajo
* Iniciar git, agregar cambios (add), anotar cambios (commit), agregar ramas, push, etc.

# Taller 
1. Crear carpeta en el *Escritorio* **tallerGitNombre**
2. Crear archivo **plantasCompartidasNombre.txt**
    + Hacer lista de 4 plantas favoritas
    + Guardar archivo
3. Abrir linea de comandos de Git (Windows) (Linux / Mac abrir la terminal)
    + Ir a la carpeta: 

>   "cd direccion/carpeta/"

+ Escribir:
```
git status
git init
git status (de nuevo)
git add *<archivo>*
git commit -m "un comentario" **ATENCIÓN**
```
4. Editar documento
    + Ver diferencias entre los archivos
>    git diff <archivo>
+ Commit
>     git add <archivo>
>     git commit -m "agregué plantas comestibles"

![Lo hicimos: Staging area](/home/jose/Documents/R_TALLER/tallerGitUNA)
5. Agregar archivo a la carpeta
    + Agregar itemes al archivo

>     git add <archivo>     ó       < . >

+ Agreguen el archivo al git
+ Revisar historial 

>     git log


