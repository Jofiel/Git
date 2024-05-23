# Crear repositorio desde un directorio

1. Navegamos al directorio de nuestro proyecto:<br> **>cd/Mi proyecto**
2. Inicializamos nuestro repositorio git (ya creado):<br> **>git init**
3. Preparamos nuestro proyecto al stage:<br> 
**>git add .**
4. Tomamos una "foto" de nuestro proyecto:<br> **>git commit -m "Comentario"**
5. Creamos nuestro repositorio en **Git Hub** copiamos el path.
6. Añadimos el origen remoto (solo la primera vez):<br> **>git remote add origin https://github.com/Jofiel/Cuadros-de-Mando.git**
7. Empujamos los cambios al repositorio remoto:<br> **git push -u origin master** <br>(si nuestro branch es main hay que cambiarlo).

### Notas:

**git init:** <br> 
<p style="margin-left: 30px;"> Crea un sub-directorio llamado .git en el directorio donde se ejecuta el comando. Este sub-directorio contiene todos los metadatos y objetos necesarios para crear el repositorio git. 

# ¿Qué significan las letras en el explorador de archivos?

Las letras que aparecen junto a los archivos en el explorador de archivos en (VS Code) indican el estado de los archivos en relación con el control de versiones de Git.

1. **U - Untracked (No rastreado):**<br> 
-El archivo es nuevo y Git no lo esta rastreando todavia.<br>
-Si queremos que Git lo comience a rastrear este archivo, se debe añadir al stage, con **git add nombre_archivo**

2. **M - Modified (Modificado):**<br>
-El archivo ha sido modificado desde el ultimo commit.<br>
-Si deseamos guardar los cambios en el proximo commit, debemos añadir estos cambios al indice **stage** usando **git add.**

3. **A - Added (Añadido al Stage)**<br>
-El archivo ha sido añadido al Stage y esta listo para ser incluido en el proximo commit.
-Para guardar los cambios en el repositorio debemos hacer solo un commit.



