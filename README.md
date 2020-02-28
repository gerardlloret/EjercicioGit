# Actividad 2: Introducción a Git
## Memoria
1. Lo primero que tenemos que hacer es ir a Github y crear un nuevo repositorio indicándole que queremos que sea un repositorio privado.  
![Imagen1](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/crearRepositorio.png)
2. Luego pulsamos en Clone para clonar el repositorio en local.  
![Imagen2](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/clonarRepo.png)
3. Vamos a la carpeta donde queremos clonar nuestro repositorio y usamos el comando “git clone” junto a la url que hemos clonado.  
![Imagen3](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/gitClone.png)
4. Luego vamos a indicar a git quien somos con el comando “git config --global” más el nombre y el email.  
![Imagen4](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/IndicarUsuario.png)
5. Ahora añadimos el fichero de Word que usaremos para la práctica en nuestro repositorio local.  
![Imagen5](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/wordEnLocal.png)
6. Para agregarlo al repositorio remoto tendremos que usar primero el comando “git add .”, para añada todos los archivos nuevos en el siguiente commit.  
Luego haremos “git commit -a -m” junto a un mensaje y finalmente “git push origin master” para subir el archivo al repositorio.  
![Imagen6](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/primerPush.png)
7. Luego vamos a modificar el Word en local, una vez modificado haremos un commit y un push de la misma forma que en el paso anterior.  
![Imagen7](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/primerCambio.png)
8. Para revisar los cambios que se hayan realizado en el último commit usaremos el comando “git log -p -1”. Con esto podemos ver las líneas que ya teníamos y las que se han agregado.  
![Imagen8](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/comprobarPrimerCommit.png)
9. A continuación, invitamos a un colaborador para que realice algún commit en nuestro archivo.  
![Imagen9](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/colaborador.png)
10 .Una vez lo haya modificado usaremos el comando “git pull” para descargar los cambios.  
![Imagen10](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/gitPull.png)
11. Al igual que hicimos anteriormente podemos comprobar que ha cambiado con “git log -p -1”.  
![Imagen11](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/comprobarCommitColaborador.png)
12. Ahora vamos a crear una carpeta que contendrá archivos personales que llamaremos “personal”.  
No queremos que esta carpeta se sincronice con nuestro repositorio por lo que tendremos que crear un fichero “.gitignore” y añadirle la ruta a la carpeta.  
Como en Windows no podemos crear un fichero sin nombre primero vamos a crearlo como un txt.  
![Imagen12](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/crearGitignore.png)
13. Una vez creado usaremos el comando “ren” para renombrarlo, con la extensión que nos interesa.  
![Imagen13](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/renombrarGitIgnore.png)
14. Lo siguiente que haremos será realizar un tercer cambio para posteriormente borrarlo.  
Para eso vamos a hacer una modificación de la misma forma en que lo habíamos hecho anteriormente.  
![Imagen14](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/tercerCambio.png)
15. Para borrar el último commit usamos el comando “git reset --hard HEAD~1” y para deshacer el push haremos “git push origin HEAD --force”.  
![Imagen15](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/deshacerCommitPush.png)
16. Por último, usamos el comando “git log” para ver los todos los commits realizados y comprobar como efectivamente se ha borrado el comit que habíamos hecho.  
![Imagen16](https://raw.githubusercontent.com/gerardlloret/EjercicioGit/tree/master/imagenes/gitLogFinal.png)
