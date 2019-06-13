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
5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
6. ¿Qué comando o comandos utilizaste en el paso 25?
7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
8. ¿Qué comando o comandos utilizaste en el paso 27?
9. ¿Qué comando o comandos utilizaste en el paso 28?
10. ¿Qué comando o comandos utilizaste en el paso 29?
11. ¿Qué comando o comandos utilizaste en el paso 30?
12. ¿Qué comando o comandos usaste en el paso 32?
13. ¿Qué comando o comandos usaste en el punto 33?