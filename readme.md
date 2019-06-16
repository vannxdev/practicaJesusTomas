## Práctica de Jesús Tomás Botella

1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?

    Para deshacer el último *commit* y perder los datos del working copy use el comando:

    ```
    git reset --hard HEAD~1
    ```
    Si hubiese usado el comando sin poner `--hard`, no habría borrado el trabajo realizado en el working copy.

2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

    Primero he utilizado el comando `git reflog` para poder ver los ids de los comits y buscar al que quiero ir. A continuacion he utilizado el siguiente comando para ir al commit deseado.
    ```
    git reset --hard 8d6c435
    ```
    
3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

    Al hacer `git merge master` me dice que *Already up-to-date*, esto quiere decir que no hay nada que copiar de master. Si se usa el comando `gitk` se abre una ventana en la que aparecen bastantes datos y se puede ver el grafo y donde esta cada rama, como era de esperar, la rama *master* esta por debajo de *styled*.
    
4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

    Si que causo un conflicto. Se produjo el conflicto porque el mismo archivo esta distinto en los dos sitios, y git no decide cual quiero, nos dice que lo solucionemos y luego hagamos el commit para indicar que se ha resuelto.
    
5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

    No ocasionó ningun conflicto, segun el informe despues de hacer el merge, se hizo "fast-forward" y se añadio el archivo readme.md y se modificó el archivo git-nuestro.md.
    
6. ¿Qué comando o comandos utilizaste en el paso 25?

    Utilice el comando `git log --graph`, se podrían usar otros para verlo más compacto, pero con este me muestra mejor la informacion de cada commit.

7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

    No, porque se quiere mantener el trabajo de la rama master y adquirir el trabajo de la rama title.

8. ¿Qué comando o comandos utilizaste en el paso 27?

    Use el comando `git reset HEAD~1` para volver al commit anterior sin perder los cambios en el working copy, para perder los cambios en el working copy habria que hacer `git reset --hard HEAD~1`

9. ¿Qué comando o comandos utilizaste en el paso 28?

    Para descartar cambios, git te ofrece una pequeña ayuda cuando haces `git status` despues de efectuar el merche, y el comando utilizado para descartar los cambios es: `git checkout -- git-nuestro.md`

10. ¿Qué comando o comandos utilizaste en el paso 29?

    Se ha utilizado el comando `git branch -D title`

11. ¿Qué comando o comandos utilizaste en el paso 30?

    Primero se usa el comando `git reflog` para buscar la id del commit del merge, copiamos el id, y luego hacemos un `git reset --hard <id_commit>`

12. ¿Qué comando o comandos usaste en el paso 32?

    Primero se usa el comando `git reflog` para buscar la id del primer commit, copiamos la id y usamos `git reset --hard 171cfc8`

13. ¿Qué comando o comandos usaste en el punto 33?

    Primero se usa el comando `git reflog` para buscar la id del último commit, copiamos la id y usamos `git reset --hard 2073e77`