![](https://github.com/joselatrans/tallerGit/blob/master/imagenes/Heredia.jpg?raw=true)
![](https://github.com/joselatrans/tallerGit/blob/master/imagenes/git1.gif?raw=true)

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

![La historia](https://github.com/joselatrans/tallerGit/blob/master/imagenes/conejo.png?raw=true)

1. Crear carpeta en el *Escritorio* **tallerGit<SuNombre>**
2. Crear archivo **plantasCompartidas<SuNombre>.txt**
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
git add <archivo>
git commit -m "un comentario" **ATENCIÓN**
```
4. Editar documento
    + Ver diferencias entre los archivos
>    git diff <archivo>	(--staged)
+ Commit
>     git add <archivo>
>     git commit -m "agregué plantas comestibles"

![Lo hicimos: Staging area](https://github.com/joselatrans/tallerGit/blob/master/imagenes/git-staging-area.png?raw=true)

5. Agregar archivo a la carpeta
    + Agregar itemes al archivo

>     git add <archivo>     ó       < . >

+ Agreguen el archivo al git
+ Revisar historial 

>     git log

### Diferencias?

![Control de versiones](https://github.com/joselatrans/tallerGit/blob/master/imagenes/git-checkout.png?raw=true)

```
git diff HEAD~1 <archivo>
```
> checkout

Checkout es un comando que nos permite volver a la versión que está bien, en caso de que hayamos guardado y "giteado" un error terrible.

### Ignorando cosas
En un git no siempre es conveniente subir todo lo que tenemos en la carpeta.

Git hace una copia de **todos** los archivos en esa carpeta, debemos de mantenerla liviana.

> .gitignore

Es un archivo que sirve para decirle a Git que no queremos que copie

1. Cree algunos archivos
2. Cree un .gitignore
3. Ponga el nombre de los archivos en el .gitignore
4. Gitee la carpeta

¿Qué pasa si "giteamos" los archivos y luego los metemos en el .gitignore?

- Extra: 
1. Cree archivos d1.dat, d2.dat, d3.dat
2. Metalos en el .gitignore con <*.dat>
3. Gitee :metal:

## Colaboración
![Repositorios](https://github.com/joselatrans/tallerGit/blob/master/imagenes/comparativa-git.png?raw=true)

[Github](https://github.com/) es más famoso, pero [Gitlab](https://about.gitlab.com/) es completamente open source y además permite hacer repositorios privados de forma gratuita, para Github hay que pagar o poner el correo institucional (2 años). 

Sin embargo...

1. Haga un cuenta en **Github**.
	+ Si ya tiene logueese

2. Logueese en su cuenta

![Repositorios de Git](https://github.com/joselatrans/tallerGit/blob/master/imagenes/git_repositories.png?raw=true)

1. Haga un repositorio nuevo en su cuenta.

> git remote add origin <link>

> git push -u origin master

![](https://github.com/joselatrans/tallerGit/blob/master/imagenes/pushRun.jpeg?raw=true)

### Ramificaciones
![Branches](https://github.com/joselatrans/tallerGit/blob/master/imagenes/branches_git.png?raw=true)

> git branch

> git remote -v

#### Trabajo en grupo

1. Haga una carpeta nueva que se llame **gitColaboracion**

2. Vaya a esa carpeta en la linea de comandos de Git

> git clone <link>

3. Añadan a su colaborador

#### ¿Sin conflictos o con conflictos?

```
git push
git pull
```
![Catdog](https://github.com/joselatrans/tallerGit/blob/master/imagenes/catdog.jpg?raw=true)

Cada vez que un colaborador haga **cambios** y los suba el otro debe de usar **pull** si **no** lo hace van a haber **conflictos**

Lo bueno es que se pueden resolver fácil :chicken:

1. Hagan cambios los dos y sin hacer **pull** hagan **push**

En caso de ser necesario:

> git push --force origin master 

2. Ahora el "dueño" arregle los cambios y los sube 
3. El colaborador haga **pull**
4. Edite el documento
5. Suba los cambios
6. Revisen

# Integración con RStudio

![](https://github.com/joselatrans/tallerGit/blob/master/imagenes/joke.png?raw=true)

Ruta para configuración:
  
  Tools --> Global options... --> Git/SVN
  
**Se usa para proyectos**

#### Ejercicio

1. Cree un proyecto en RStudio de la carpeta *tallerGit<SuNombre>*
  
  1.2. Explórelo
  
2. Cree un proyecto en RStudio
  
  2.1. Hágale un repositorio Git desde RStudio

:metal:

## Recursos

[Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)

Presentaciones base para el taller
Filipe Fernandes
[1](https://jiffyclub.github.io/2015-07-06-scipy/slides-local_version_control.html#/5)
[2](http://slides.com/abostroem/collaborating_using_git#/)
[3](http://slides.com/abostroem/deck-4#/)
![](https://www.acrl.ala.org/ULS/wp-content/uploads/2018/04/software-carpentry.png)

[Más sobre ramificaciones](https://gerardnico.com/code/version/git/branch)

# Institución
![](http://www.documentos.una.ac.cr/bitstream/handle/unadocs/1684/UNA1LINE.JPG?sequence=3&isAllowed=y)
![](http://www.exactasynaturales.una.ac.cr/images/logos/cienciasbiologicas.jpg)

