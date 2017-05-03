Git Basics
==========

index
-----
- [Git command](#git-command)
    - [Git clone](#)
    - [Git fetch](#)
    - [Git merge](#)
    - [Git pull](#)
    - [Git commit -a](#)
    - [Git add (-u)](#)
    - [Git push](#)
    - [Git diff](#)
    - [Git diff head](#)
- Git stash
- Git WorkFlow

-----

### Git command

#### git clone :
  Este comando se utiliza solo una vez al inicio para descargar el proyecto
  y siempre que se corre se le debe pasar el path o url de descarga del repositorio remoto del proyecto.
  ```bash
  git clone http://baseProyectOwner.com/url/path/proyecyGroup/_git/MyProyect
  ```
#### git fetch :
  Con `git fetch` descargamos todos los cambios que se hayen en nuestro repositorio remoto a nuestro repositorio local, lo cual representa un paso intermedio, evitando asi traer cambios directamente a nuestro directorio de trabajo, y ahorrando asi posibles conflictos de mergeo. entendiendo esto, unforma de ejecutar esto seria primero correr el comando `git fetch`, y luego un `git diff head`
#### git merge :
  Merges one or more branches into your current branch and automatically creates a new commit if there are no conflicts. Example: git merge newbranchversion
#### git pull :
  Fetches the files from the remote repository and merges it with your local one. This command is equal to the git fetch and the git merge sequence. Example: git pull origin
#### git commit -a :
  Takes all of the changes written in the index, creates a new commit object pointing to it and sets the branch to point to that new commit. Examples: git commit -m ‘committing added changes’
  ```
    git commit -a -m "committing all changes, equals to git add and git commit"
  ```
#### git add (-u) :
  Adds files changes in your working directory to your index.
  you can add a single file, a folder or allExample:
  ```
  git add rootPath/fileFolder/subfolder/index.js
  git add rootPath/fileFolder/subfolder/*.js
  git add rootPath/fileFolder/*
  git add .
  ```
#### git push :
  Pushes all the modified local objects commited in your local repository to the remote repository and advances its branches. Example:
  ```
    git push origin currentWorkingBranch
  ```
#### git diff :
  Compare your lost file changes in your working directory, with the last changes added to stage
  Generates patch files or statistics of differences between paths or files in your git repository, or your index or your working directory. Example: git diff
#### git diff head :

![alt text](./img/git-comand-flow-schema.png "git comand flow schema")

----

![alt text](./img/git-stash-schema-A.png "git stash schema-A")

----

![alt text](./img/git-stash-schema-B.png "git stash schema-B")
