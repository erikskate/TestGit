#Curso de _Git_ & _GitHub_

Hola Soy erik y estoy en un curso para aprender GIT.

COMANDOS GIT

// INICIAR UN REPOSITORIO EN GIT
git init 

//Pasar los archvios al staged
git add .

//comando para hacer commit
git commit -m "descripcion del cambio"

//CREAR EL REPO EN GIT Y CREAR EL ORIGEN 
git remote add origin https://github.com/erikskate/TestGit.git

//HACER MI PRIMER PUSH EN LA RAMA MASTER
git push -u origin master

PARA REMPLAZAR la rama master por main en GitHub
1# Crea la rama local main y pasale el historial de la rama master
git branch -m master main

2# Haz un push de la nueva rama local main en el repo remoto de github
git push -u origin main

3# Cambia el HEAD actual a la rama main
git symbolic-ref refs/remotes/origin/HEAD refs/remotes/origin/main

4# Cambiar la rama default de master a main en tu repo de git
git push origin --delete master