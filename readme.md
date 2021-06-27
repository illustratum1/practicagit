Práctica del curso de git, gitHub y Sourcetree
Información de contacto del profesor:
Alberto Casero acasero@agbotraining.com Skype: kas.appeal
Twitter: @KasAppeal

Alumno: Antonio López Oliveros
illustratum01@gmail.com

Ejercicio 1:

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

git reset --hard HEAD~1

He hecho un git reset para deshacer el último commit (por eso puse HEAD~1).
Lo he hecho HARD para perder los cambios realizados en el working copy al crear el commit antes.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

git reflog                    -- lo he usado para localizar el id del commit que quiero rehacer
git reset --hard idCommit     -- Lo he hecho HARD para aplicar los cambios realizados en el working copy en ese commit.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

Si, porque había modificado el archivo git-nuestro.md en la rama styled.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si, porque había modificado el archivo git-nuestro.md en la rama htmlify.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

Si, porque había modificado el archivo git-nuestro.md en la rama styled.

- ¿Qué comando o comandos utilizaste en el paso 25?

git log --graph

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

No, porque había hecho cambios en git-nuestro(había añadido el título).
Sólo puede haber conflictos en un merge no fast-forward.

- ¿Qué comando o comandos utilizaste en el paso 27?

git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?

git reflog                    -- lo he usado para localizar el id del commit donde estoy al hacer el paso 27.
git reset --hard idCommit     -- Lo he hecho HARD para descartar los cambios realizados en el working copy en el merge antes.


- ¿Qué comando o comandos utilizaste en el paso 29?

git branch -D title           -- Debo hacerlo con -D porque dejaba commits inalcanzables.

- ¿Qué comando o comandos utilizaste en el paso 30?

git reflog                    -- lo he usado para localizar el id del commit cuando hicimos el merge
git reset --hard idCommit     -- Lo he hecho HARD para aplicar los cambios realizados en el working copy en ese commit.

- ¿Qué comando o comandos usaste en el paso 32?

git reflog                    -- lo he usado para localizar el id del primer commit
git reset --hard idCommit     -- Lo he hecho HARD para aplicar los cambios realizados en el working copy en ese commit.

- ¿Qué comando o comandos usaste en el punto 33?

git reflog                    -- lo he usado para localizar el id del commit en que pusimos título al poema
git reset --hard idCommit     -- Lo he hecho HARD para aplicar los cambios realizados en el working copy en ese commit.


Ejercicio 2:

La práctica consiste en hacer un fork del repositorio https://github.com/kasappeal/nerdquotes.git y, en el archivo README.md añadir, en formato markdown ,
una cita (a ser posible con connotaciones frikis) seguido del nombre de su autor (en cursiva).
Cada alumno deberá introducir su cita en una posición aleatoria entre dos frases ya existentes (por favor no la pongáis todos al final o al principio,
que luego me toca resolver conflictos!).

He enviado dos comentarios porque vi que en tu repo no aparecía en pull requests(igual no se había actualizado la inforamción)
