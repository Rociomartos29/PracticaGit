**- ¿Qué comando utilizaste en el paso 11? ¿Por qué?**
    Primero he usado "git reset HEAD~1" para volver al commit anterior y  a continuación he usado "git restore git-nuestro" para volver a la versión anterior del alrchivo.


**- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**
    Primero realizo un "git reflog" para ver todos los commits por los que ha pasado Head. A continuación uso "git reset --hard a1eba46" para devolver los cambios que había realizado. Hago un "git log" para asegurarme de que el commit vuelve a aparecer.

**- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
    No me ha causado conflicto. Me encuentro en la rama Styled y al realizar el merge a main me ha salido el mensaje "Already un to date" así que he realizado "git checkout" para cambiar de rama a main y hacer el merge desde ahí y al hacerlo se me han hecho los cambios que tenía en la rama Styled en la rama main.

**- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
    No me ha causado ningun conflicto. Me ha pasado igual que en el anterior.

**- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
    Al cambiar a la rama main me sale el mensaje d eque el flujo ascendente desapareció y he usado "git branch --unset-upstream" para arreglarlo. Al hacer el merge no me ha causado conflicto.

**- ¿Qué comando o comandos utilizaste en el paso 25?**
    Utilizo "git log --graph

**- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
    Uso "git merge --no-ff title " y me sale el editor de texto. Se me hace correctamente. También puede realizarse Fast Forward.

**- ¿Qué comando o comandos utilizaste en el paso 27?**
    Para encontrar el merge hago un "git reflog". He encontrado la referencia y uso "git revert -m 1 --no-commit b52e6f1" que deshace el commit del merge y el "--no-commit" hace que no se vuelva a crear un commit. Después utilizo "git stash" para mantener los cambios en el area de trabajo.

**- ¿Qué comando o comandos utilizaste en el paso 28?**
    Uso "git reset --hard HEAD".

**- ¿Qué comando o comandos utilizaste en el paso 29?**
    Utilizo "git branch -d title".

**- ¿Qué comando o comandos utilizaste en el paso 30?**
    Para empezar realizo un "git reflog" para identificar el merge. Después uso "git merge --no-ff b52e6f1".

**- ¿Qué comando o comandos usaste en el paso 32?**
    He usado "git reset 90b1475" y "git reflog" para identificar el primer commit.

**- ¿Qué comando o comandos usaste en el punto 33?**
    Vuelvo a empezar con un "git reflog", identifico el commit y utilizo "git reset --hard ca75dca". Creo la rama de nuevo con "git branch title ca75dca.
