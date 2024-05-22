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