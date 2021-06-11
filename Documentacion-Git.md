# Documentando con Alberto
## Laboratorio01 GIT

>Elementos necesarios para el desarrollo del Laboratorio01:

- Ubuntu version 20.04.2.0 (puede ser una version inferior o superior)
- GIT version 2.24.0. (puede ser una version inferior o superior)

Pasos a seguir para la creacion del Laboratio01 Docker:

>1. Realizamos la configuracion GIT para poder ver que de aqui en adelante cualquier modificacion que hagamos tenga nuestro nombre
`````
git config --global user.name "Alberto Urquiza"
git config --global user.email "aurquiza@everis.com"

"Para poder validarlo ejecutamos el comando"

git config --list

`````
>2. Ejecutamos el siguiente comando para que nuestro repositorio sea manejado por GIT
`````
git init 

Initialized empty Git repository in /home/alberto/Laboratorio01/.git

`````
>3. Si queremos crear archivos y que no sea supervisado por GIT ejecutamos el comando.
`````
.gitignore

"Adentro de este archivo podemos colocar lo que no queramos que supervise GIT"
`````
>4. Para ver el estado de nuestros archivos y en que rama nos encontramos
`````
git status 

"Aqui podemos monitorear que archivos  estan en seguimiento o no por GIT"

`````
>5. Para poder agregar estos archivos que no estan siendo seguidos por GIT
`````
git add <nombre del archivo>

En la rama v15-albertov15
Cambios no rastreados para el commit:
  (usa "git add <archivo>..." para actualizar lo que será confirmado)
  (usa "git restore <archivo>..." para descartar los cambios en el directorio de trabajo)
	modificado:     src/index.php

`````
>6. Para validar que han sido agregados de manera correcta
`````
git status

En la rama v15-albertov15
Cambios a ser confirmados:
  (usa "git restore --staged <archivo>..." para sacar del área de stage)
	modificado:     src/index.php

`````
>7. Guardamos todos los cambios hechos en el staging area , junto con una breve descripcion commit que hayamos realizado 
`````
git commit -m "Se cambio la version 01 a version 02"

`````
>8. Validamos que se a ejecutado de manera correcta , visualizamos el historial
`````
git log 

commit b5fe18e433c193d39bf625970ffabf7c60c577c3 (HEAD -> v15-albertov15)
Author: Alberto <aleduurna@gmail.com>
Date:   Fri Jun 11 10:27:04 2021 -0500

    Se cambio la version 01 a version 02

`````
>9. Finalmente subimos los cambios realizados al repositorio GitHub
`````
git push origin main 

`````
>10. Nos logueamos con nuestra cuenta de GitHub y validamos en nuestro repositorio web la rama y los cambios efectuados
`````
"https://github.com/Beto9730/Laboratorio01.git"

`````



