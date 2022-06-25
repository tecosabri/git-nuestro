**¿Qué comando utilizaste en el paso 11? ¿Por qué?**
	
`git reset --hard HEAD~1`

El último commit es la última operación realizada. Al utilizar `HEAD~1` estamos indicando que el `reset`se refiere únicamente a la última operación. Además, mediante `--hard` provocamos que se descarten todos los cambios realizados en el *working copy* desde el `commit`.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reset --hard 7034798`

`7034798`es la referencia en la que se efectúa el `commit` con el que damos estilo al archivo. Por lo tanto, este comando nos lleva al estado del repositorio en el que se le ha dado estilo al archivo y se recupera el *working copy* tal y como se encontraba en ese momento.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

`git merge master`

Este merge no puede ocasionar conflictos porque la rama *styled* ya contiene todos los cambios de la rama *master*.


**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

El documento *git-nuestro.md* de *htmlify* ha sufrido cambios que no conoce la rama *styled*. Estas modificaciones se han producido sobre las mismas líneas del documento, con lo que se produce un conflicto al hacer el `merge`.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No ha causado ningún conflicto porque en master no se ha hecho ningún cambio desde que *styled* se separase.

**¿Qué comando o comandos utilizaste en el paso 25?**

`git log --all --decorate --oneline --graph`

He utilizado el comando con `--all`para ver el gráfico completo, con el último commit del título.

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Podría ser fast forward porque la rama *master* y *title* formaban una lista.

**¿Qué comando o comandos utilizaste en el paso 27?**

`git reset HEAD~1`

Sin la opción `--hard`se mantienen los cambios del working copy.


**¿Qué comando o comandos utilizaste en el paso 28?**

`git checkout -- git-nuestro.md`

**¿Qué comando o comandos utilizaste en el paso 29?**

`git branch -D title`

**¿Qué comando o comandos utilizaste en el paso 30?**

`git reflog`

Buscamos la referencia del merge (464d38d)

`git reset --hard 464d38d`

Volvemos al estado del repositorio en el que se había hecho el merge.

**¿Qué comando o comandos usaste en el paso 32?**

`git reset --hard f8e35fc9579cf109804f5deafad0fba7113f4ac5`

f8e35fc9579cf109804f5deafad0fba7113f4ac5 es la referencia del primer `commit`.

**¿Qué comando o comandos usaste en el punto 33?**

`git reset --hard 40df191`

40df191 es la referencia del `commit`en el que se le da título al documento.