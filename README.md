# Actividad 2: Introducción a Git
## Memoria
1. Lo primero que tenemos que hacer es ir a Github y crear un nuevo repositorio indicándole que queremos que sea un repositorio privado. 
![crearRepositorio](https://user-images.githubusercontent.com/58988814/75556753-15004480-5a3f-11ea-8761-60c22bf956d7.PNG)
2. Luego pulsamos en Clone para clonar el repositorio en local.  
![clonarRepo](https://user-images.githubusercontent.com/58988814/75556785-22b5ca00-5a3f-11ea-8efd-90c569f813c4.PNG)
3. Vamos a la carpeta donde queremos clonar nuestro repositorio y usamos el comando “git clone” junto a la url que hemos clonado.  
![gitClone](https://user-images.githubusercontent.com/58988814/75556802-2fd2b900-5a3f-11ea-9027-0d3b262bc958.PNG)
4. Luego vamos a indicar a git quien somos con el comando “git config --global” más el nombre y el email.  
![IndicarUsuario](https://user-images.githubusercontent.com/58988814/75556845-40832f00-5a3f-11ea-8786-cbf1c430fc05.PNG)
5. Ahora añadimos el fichero de Word que usaremos para la práctica en nuestro repositorio local.  
![wordEnLocal](https://user-images.githubusercontent.com/58988814/75556914-601a5780-5a3f-11ea-8d6c-687e23a3a71d.PNG)
6. Para agregarlo al repositorio remoto tendremos que usar primero el comando “git add .”, para añada todos los archivos nuevos en el siguiente commit.  
Luego haremos “git commit -a -m” junto a un mensaje y finalmente “git push origin master” para subir el archivo al repositorio.  
![primerPush](https://user-images.githubusercontent.com/58988814/75556971-7e805300-5a3f-11ea-8820-ac05cfe23161.PNG)
7. Luego vamos a modificar el Word en local, una vez modificado haremos un commit y un push de la misma forma que en el paso anterior.  
![primerCambio](https://user-images.githubusercontent.com/58988814/75557005-8fc95f80-5a3f-11ea-85f4-1e6ebf1dfd3d.PNG)
8. Para revisar los cambios que se hayan realizado en el último commit usaremos el comando “git log -p -1”. Con esto podemos ver las líneas que ya teníamos y las que se han agregado.  
![comprobarPrimerCommit](https://user-images.githubusercontent.com/58988814/75557049-a2dc2f80-5a3f-11ea-9fad-2845e008636b.PNG)
9. A continuación, invitamos a un colaborador para que realice algún commit en nuestro archivo.  
![colaborador](https://user-images.githubusercontent.com/58988814/75557085-b38ca580-5a3f-11ea-9aeb-87ce1df5207f.PNG)
10. Una vez lo haya modificado usaremos el comando “git pull” para descargar los cambios.  
![gitPull](https://user-images.githubusercontent.com/58988814/75557128-c4d5b200-5a3f-11ea-83f3-cc09409f481a.PNG)
11. Al igual que hicimos anteriormente podemos comprobar que ha cambiado con “git log -p -1”.  
![comprobarCommitColaborador](https://user-images.githubusercontent.com/58988814/75557168-d61ebe80-5a3f-11ea-95a2-f38aad3a7ca4.PNG)
12. Ahora vamos a crear una carpeta que contendrá archivos personales que llamaremos “personal”.  
No queremos que esta carpeta se sincronice con nuestro repositorio por lo que tendremos que crear un fichero “.gitignore” y añadirle la ruta a la carpeta.  
Como en Windows no podemos crear un fichero sin nombre primero vamos a crearlo como un txt.  
![crearGitignore](https://user-images.githubusercontent.com/58988814/75557207-e9ca2500-5a3f-11ea-9ade-ded2a6cd4664.PNG)
13. Una vez creado usaremos el comando “ren” para renombrarlo, con la extensión que nos interesa.  
![renombrarGitIgnore](https://user-images.githubusercontent.com/58988814/75557247-f51d5080-5a3f-11ea-9985-d7d2649b2b70.PNG)
14. Lo siguiente que haremos será realizar un tercer cambio para posteriormente borrarlo.  
Para eso vamos a hacer una modificación de la misma forma en que lo habíamos hecho anteriormente.  
![tercerCambio](https://user-images.githubusercontent.com/58988814/75557344-2433c200-5a40-11ea-9e00-2f503129fbbd.PNG)
15. Para borrar el último commit usamos el comando “git reset --hard HEAD~1” y para deshacer el push haremos “git push origin HEAD --force”.  
![deshacerCommitPush](https://user-images.githubusercontent.com/58988814/75557469-59401480-5a40-11ea-957a-7120f528fe97.PNG)
16. Por último, usamos el comando “git log” para ver los todos los commits realizados y comprobar como efectivamente se ha borrado el comit que habíamos hecho.  
![gitLogFinal](https://user-images.githubusercontent.com/58988814/75556070-cd2ced80-5a3d-11ea-8138-e2f4b3d750d2.PNG)
