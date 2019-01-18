1. Tienes que modificar la escena 5 de Hamlet en el fichero scene-5.txt. En dicha escena Hamlet encuentra al fantasma de su padre. Añade este texto al fichero:

Creamos un directorio mkdir Examen
Nos movemos al directorio cd Examen
Clonamos el repositorio git clone https://github.com/IESJacaranda/deshaciendo-cambios-y-gestion-de-ramas-Kurtgon
Editamos el fichero scene-5.txt nano scene-5.txt y añadimos las nuevas líneas.

> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting flames
> Must render up myself.

2. Añade scene-5.txt al área de preparación.

git add scene-5.txt

3. Haz un commit con los cambios con un buen mensaje de commit.

git commit -m "Añadiendo nuevas lineas al fantasma"

4. Modifica las palabras del fantasma. Aquí tienes una sugerencia divertida:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting balloons
> Must render up myself.

cambiamos la palabra "balloons" con el editor nano scene-5.txt

5. Devuelve el fichero al estado del último commit.

git reset --soft scene-5.txt

6. Cambia el nombre de LARRY por LAERTES en los ficheros scene-3.txt y scene-7.txt.

nano scene-3.txt
nano scene-7.txt

7. Añade los ficheros al área de preparación usando un único comando git.

git add scene-3.txt && git add scene-7.txt

8. Vamos a cometer un error a propósito. Borra cualquier línea del fichero scene-2.txt.

nano scene-2.txt (y borramos la primera linea)

9. Añade scene-2.txt al área de preparación.

git add scene-2.txt

10. Comprueba el estado del repositorio. 

git status

11. Devuelve scene-2.txt al directorio de trabajo.

git checkout scene-2.txt

12. Haz un commit para guardar los cambios realizados en el nombre de Larry por Laertes.

git commit -m "Hemos cambiado el nombre Larry por Laertes"


13. Busca el primer commit que has hecho y vuelve a dicho commit. Indica como has buscado el commit anterior y como has vuelto a él.


14. Crea una nueva rama llamada **reinventando_hamlet**
 
 git branch reinventado_hamlet

15. Cámbiate a dicha rama

git checkout reinventado_hamlet

16. Mejora la escena 2 como creas conveniente.

nano scena-2.txt Ghost: Come here baby!!!

17. Haz un commit con los cambios con un mensaje adecuado.

git commit -m "El fantasma tiene nueva frase"


18. Vuelve a la rama master.

git checkout master

19. Elimina la rama **reinventando_halet**

git branch -d reinventando_halet

20. Crea una nueva rama, modifica algo en la rama master, haz commit y llévate los cambios a la rama que has creado.
21. Provoca un conflicto entre la rama master y la rama que has creado (indica lo que has hecho). Une la rama a la rama master resolviendo el conflicto.
