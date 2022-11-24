# Práctica del Módulo Git

######  Apunte: Si ves en alguna pregunta con varios comandos de Git, están ordenados por orden de aplicación. 


## :point_right: 1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?

```
git reset --hard HEAD~1
```
- Porque queremos deshacer el último commit y perder los cambios realizados en el Working Copy.


## :point_right: 2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
```
git reflog
```
- Porque queremos conocer el HASH del commit que quiero rehacer.
```
git reset HASH
```
- Se utiliza este comando + HASH que hemos obtenido del reflog porque queremos restaurar ese commit en específico. 
```
git status
```
- Porque he querido comprobar que todo estaba al día.

## :point_right: 3. El merge del paso 13, ¿Causó algun conflicto? ¿Porqué?

- Ha aparecido este mensaje *Already up to date* al realizar el merge debido a que la rama que se absorbe ya se encuentra actualizada (styled absorbe a master) 

## :point_right: 4. El merge del paso 19, ¿Causó algun conflicto? ¿Porqué?

- Ha causado el conflicto *Merge conflict in git-nuestro.md Automatic merge failed; Fix conflicts and then commit the result* debido a que las dos ramas tenían el mismo archivo (git-nuestro.md) pero con un contenido diferente. Para solucionar este conflicto y quedarnos con el contenido de la rama styled, utilizamos el comando *nano git-nuestro.md* para abrir el editor de nano + el nombre del archivo y nos quedamos con el contenido de styled.

## :point_right: 5. El merge del paso 21, ¿Causó algún conflicto? ¿Porqué?

- No he tenido ningún conflicto, ya que Git ha realizado un merge de tipo fast forward

## :point_right: 6. ¿Qué comando o comandos utilizaste en el paso 25?
```
git log --graph
```

## :point_right: 7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

- No podría ser fast forward porque ambas ramas se sitúan a modo bifurcación y por tanto si lo hiciesemos de tipo fast forward nos daría un conflicto.

## :point_right: 8. ¿Qué comando o comandos utilizaste en el paso 27?

```
git log
```
```
git reset HEAD~1
```
## :point_right: 9. ¿Qué comando o comandos utilizaste en el paso 28?

```
git status
```

```
git restore git-nuestro.md
```
## :point_right: 10. ¿Qué comando o comandos utilizaste en el paso 29?

```
git branch -D title
```
## :point_right: 11. ¿Qué comando o comandos utilizaste en el paso 30?

```
git reflog
```
```
git reset +hash (donde pone hash es donde se incluye el hash que hemos obtenido del reflog)
```
## :point_right: 12. ¿Qué comando o comandos utilizaste en el paso 32?

```
git log
```
```
git checkout +hash 
```
## :point_right: 13. ¿Qué comando o comandos utilizaste en el paso 33?
```
git reflog
```
```
git checkout +hash 
```







