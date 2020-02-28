# Actividad 2: Introducción a Git
## Memoria
Lo primero que tenemos que hacer es ir a Github y crear un nuevo repositorio indicándole que queremos que sea un repositorio privado.
![Imagen1](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/master/imagenes/crearRepositorio.PNG)
Luego pulsamos en Clone para clonar el repositorio en local.
Foto2
Vamos a la carpeta donde queremos clonar nuestro repositorio y usamos el comando “git clone” junto a la url que hemos clonado.
Foto3
Luego vamos a indicar a git quien somos con el comando “git config --global” más el nombre y el email.
Foto4
Ahora añadimos el fichero de Word que usaremos para la práctica en nuestro repositorio local.
Foto5
Para agregarlo al repositorio remoto tendremos que usar primero el comando “git add .”, para añada todos los archivos nuevos en el siguiente commit.
Luego haremos “git commit -a -m” junto a un mensaje y finalmente “git push origin master” para subir el archivo al repositorio.
Foto6
Luego vamos a modificar el Word en local, una vez modificado haremos un commit y un push de la misma forma que en el paso anterior.
Foto7
Para revisar los cambios que se hayan realizado en el último commit usaremos el comando “git log -p -1”. Con esto podemos ver las líneas que ya teníamos y las que se han agregado.
Foto8
A continuación, invitamos a un colaborador para que realice algún commit en nuestro archivo.
Foto9
Una vez lo haya modificado usaremos el comando “git pull” para descargar los cambios.
Foto10
Al igual que hicimos anteriormente podemos comprobar que ha cambiado con “git log -p -1”.
Foto11
Ahora vamos a crear una carpeta que contendrá archivos personales que llamaremos “personal”.
No queremos que esta carpeta se sincronice con nuestro repositorio por lo que tendremos que crear un fichero “.gitignore” y añadirle la ruta a la carpeta.
Como en Windows no podemos crear un fichero sin nombre primero vamos a crearlo como un txt.
Foto12
Una vez creado usaremos el comando “ren” para renombrarlo, con la extensión que nos interesa.
Foto13
Lo siguiente que haremos será realizar un tercer cambio para posteriormente borrarlo.
Para eso vamos a hacer una modificación de la misma forma en que lo habíamos hecho anteriormente.
Foto14
Para borrar el último commit usamos el comando “git reset --hard HEAD~1” y para deshacer el push haremos “git push origin HEAD --force”.
Foto15
Por último, usamos el comando “git log” para ver los todos los commits realizados y comprobar como efectivamente se ha borrado el comit que habíamos hecho.

