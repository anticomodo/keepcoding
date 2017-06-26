1. - ¿Qué comando utilizaste en el paso 11? ¿Por qué?

git reset --hard HEAD~1
Porque tengo que ir a la posición anterior (o deshacer el commit) eliminando el working copy.

2. - ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

git checkout --
Porque como no puedo avanzar porque ya no aparece en el log, tengo que volver a ponerlo como estaba en la última "foto".

3. - El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No. Porque la rama styled tenía la misma información que la rama master, y además, tenía el archivo modificado, por lo tanto, se absorbe sin más.

4. - El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

Sí. Porque tiene el mismo archivo con líneas diferentes.

5. - El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

No. Porque la información de styled es más completa que la de master, y Git no quiere que pierdas nada, así que lo que realmente hace es llevar master al mismo sitio donde está styled.

6. - ¿Qué comando o comandos utilizaste en el paso 25?

git graph
Es el alias para git log --graph --decorate --pretty=oneline que lo he configurado con un git config alias.graph "..."

7. - El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

Sí, porque el antecesor es común para ambos.

8. - ¿Qué comando o comandos utilizaste en el paso 27?

git reset HEAD~1

9. - ¿Qué comando o comandos utilizaste en el paso 28? 

git checkout --

10. - ¿Qué comando o comandos utilizaste en el paso 29? 

git branch -D

11. - ¿Qué comando o comandos utilizaste en el paso 30? 

git reflog
git checkout para ir al commit en el que había absorbido title desde master
git checkout -b para volver a crear un puntero sobre este commit

12. - ¿Qué comando o comandos usaste en el paso 32?

git log 
git checkout primer commit

13. - ¿Qué comando o comandos usaste en el punto 33?

git reflog
git checkout al commit donde añado el titulo
git checkout a rama master

