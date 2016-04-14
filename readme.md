- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
`git reset --hard HEAD~1`

Porque este comando deshace el último commit y deja el working copy
como estaba antes

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
`git reset --hard HEAD@{1}`

Porque este comando mueve el puntero **styled** al commit anterior al ultimo comando que fue deshacerlo.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No causo conflicto, en realidad no hizo merge alguno porque ya **styled** contenia **Master**

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

Si hay conflicto porque el archivo readme.md es diferente en cada rama

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

No hay conflicto, porque master y styled estan alineados, se ejecuta un merge fast forward

- ¿Qué comando o comandos utilizaste en el paso 25?
`git log --graph --decorate --pretty=oneline`

Para mostrar el gráfico con los punteros y el texto de los commits

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

Si podría ser fast forward porque title y master estan en linea

- ¿Qué comando o comandos utilizaste en el paso 27?

Hago un 

`git reflog` 

identifico el puntero de master anterior al merge (e950369) y hago un 

`git reset e950369`
 
- ¿Qué comando o comandos utilizaste en el paso 28? 

`git checkout -- git-nuestro.md`

- ¿Qué comando o comandos utilizaste en el paso 29? 
`git branch -D title`

- ¿Qué comando o comandos utilizaste en el paso 30? 
Hago un 

`git reflog` 

identifico el puntero de master del merge (05dfa80) y hago un 

`git reset --hard 05dfa80`

- ¿Qué comando o comandos usaste en el paso 32?
Hago un 

`git reflog` 

para identificar el primer commit de todos y luego hago 

`git reset --hard 4b52bda`

- ¿Qué comando o comandos usaste en el punto 33?  
Hago un 

`git reflog` 

para identificar el puntero del merge final y luego hago 

`git reset --hard 05dfa80`