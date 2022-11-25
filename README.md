# PracticaCursoGit
Ejercicio manejo de git por la consola
- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
EL comando : git reset –hard HEAD~1:

Te permite volver a donde estaba (con el 1 “un paso atrás”), pero descartará los cambios del working copy, perdiendo los cambios realizados
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Comando : git reset 6359f19 && git restore git-nuestro.md
 Buscando en reflog conozco cuál era el id del último código y reset XXX me permite y a la rama y commit “punto” (por donde HEAD ha pasado) que me interesa.

Con restore recuperamos el commit




- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
Hagas un git merge main o git merge –no-ff main nunca se producirá un merge porque styled ya contiene los commits de main(todos)

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Nos pasamos git checkout styled a esta rama, y con git merge –no-ff htmliy aboservemos ésta.

Hay conflictos, nos quedamos con styled:
 Nano git-nuestro.md
Git add git-nuestro.md
Git commit

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
Git checkout main
Git merge styled: 1 file changed, 10 insertions(+), 10 deletions(-)
 No hay conflictos, styled tenia todos los commits de main y ha sido un merge fast forward.

- ¿Qué comando o comandos utilizaste en el paso 25?
git log --oneline --graph


- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Git merge –no-ff
Sí, ya que title contiene todos los commits de main, por lo que no habría conflictos

- ¿Qué comando o comandos utilizaste en el paso 27?
git log
git reset 4fc2c9ee6f031d53ca04c5c19e9cccfe377fe9f1


- ¿Qué comando o comandos utilizaste en el paso 28?
Git restore git-nuestro.md

- ¿Qué comando o comandos utilizaste en el paso 29?
Git branch –D title

- ¿Qué comando o comandos utilizaste en el paso 30?
Git reflog
Git reset 39da5bc
Git restore git-nuestro.md


- ¿Qué comando o comandos usaste en el paso 32?
Git log
Git reset 19e26eb7f063aecaed8b06121f2fd64ad15fac21

- ¿Qué comando o comandos usaste en el punto 33?
Git reflog
Git reset 39da5bc

