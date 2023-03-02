# JolprGit
Applica,Inc.
By Jose Lara
Version: 2023-03-02

Documentación de flujo de trabajo remoto con GIT
#
## Notas
1. Crear una organización
2. Crear un proyecto dentro de la organización
3. Si el proyecto es privado agregar a todos los colaboradores
4. Cada colaborador debe tener un Fork en su cuenta
5. Cada desarrollador debe clonar su fork a su máquina 
6. El programador debe agregar los remotos correspondientes del proyecto original
7. Se debe asegurar que todos este correcto sincronizado
8. Se creará una nueva rama para trabajar una funcionalidad
9. Una vez terminado el trabajo, el desarrollador sube (push) esa rama a su fork
10. En GitHub le aparecerá la opción de crear un Pull Request
11. Una vez creado el pull request el administrador del proyecto original lo revisará
12. Se aprueba o se rechaza el Pull Request (esto es por el administrador del proyecto)
13. Cada programador debe revisar constantemente (fetch) si no hay cambios en el proyecto original
14. Se debe eliminar las ramas que ya fueron aprobadas o rechazadas (esto lo hace cada programador en su fork)   
#
## Organización (Administrador del proyecto)

Se recomienda crear una organización que sea la propietaria del repositorio principal. A partir de dicho repositorio los miembros o colaboradores podrán hacer un fork hacia sus cuentas personales.
#
### Paso para crear una organización (Administrador del proyecto)

1. Click en tu foto perfil (Esquina superior derecha)
2. Click en Settings
3. Click Organizaciones (Meú izquierdo)
4. Click en Nueva organización
5. Elegir plan y llenar datos
#
## Creación de Fork (Programadores en sus cuentas personales de GitHub)

Para crear un fork debes iniciar sesión en GitHub y luego ingresar a la landing page del proyecto del que quieras sacar tu Frok.
#
## Como trabajar con 2 o más remotos

Listar remotos:
### `git remote -v`
#
Agregar remotos
### `git remote add [alias del remoto] https://github.com/jolpr/Jolprgit.git`

Ejemplo
### `git remote add applicademo2023 https://github.com/jolpr/Jolprgit.git`

Eliminar remotos
### `git remote remove applicademo2023`
#
## Creando Tags (Esto lo realiza el administrador del proyecto)

Es necesario entender que las etiquetas (o releases) sólo deben ser creadas a partil de la rama master como buena práctica.

Para entender como llamar o categorizar a tus versiones  te recomendamos un articulo en https://ed.team/blog/como-se-deciden-las-versiones-del-software

Ejemplo: git tag "v0.0.1"

#
## CMD
1. git branch dev
2. git branch
3. git checkout dev
4. git switch dev
5. git log --oneline --all
6. git remote -v
7. git status
8. git commit -am "add info"
9. git push origin main
10. git pull upstream dev
11. git fetch upstream
12. git branch -D agrega-colaborador create-tags  (Delte local)
13. git push origin --delete create-tags (Delete remote)
14. git stash
15. git stash list
16. git stash pop
17. git tag "v0.0.1"
