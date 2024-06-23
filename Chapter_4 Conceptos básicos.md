# Conceptos Básicos

### Repositorios:
Un repositorio Git es una base de datos que almacena toda la información necesaria para conservar y gestionar revisiones e historial de un proyecto.<br>
Un repositorio conserva una copia completa de todo el proyecto a lo largo de su vida útil.<br>
Dentro de un repositorio Git mantiene dos estructuras de datos principales, el _almacen de objetos_ y el _índice_.

1. **El almacen de objetos:**<br>
Contiene los archivos de datos originales y todos los mensajes de registro, información de autor, fechas e información necesaria para contruir cualquier version o rama del proyecto. 

2. **Indices:**<br>
Es un archivo binario temporal y dinámico que describe la estructura de directorios de todo el repositorio.<br>
Cuando se realizan cambios en Git almacena provisionalmente los cambios en el índice. Los cambios suele añadir, eliminar o modificar algún archivo o conjunto de archivos. El índice registra y conserva esos cambios, manteniendolos seguros hasta que se esta listo para confirmarlos.

### Nombres direccionables por contenido
Cada objeto del almacén de objetos tiene un nombre único que se genera al aplicar SHA1 al contenido del objeto. Cualquier pequeño cambios en un archivo hace que el SHA1 cambie. Los valores SHA1 son valores de 160 bits que normalmente se representan como un número hexadecimal de 40 dígitos, como **9da581d910c9c4ac93557ca4859e767f5caf5169**. Los usuarios de Git lo conocen como SHA1, código hash y aveces ID de objeto.<br> Una característica importante de el calculo de SHA1 es que siempre calcula el mismo identificador para contenido idéntico, independientemente de donde éste ese contenido. Por lo tanto, el ID hash SHA1 de un archivo es un identificador único global.

### Git rastrea el contenido
Git es más que un sistema de control de versiones: Git es un sistema de seguimiento de contenido. El almacén de objetos de Git se bása en el calculo hash del contenido de sus objetos, no en los nombres de los archivos o directorios. Por lo tanto cuando Git coloca un archivo en el almacén de objetos, lo hace basandose en el hash de los datos y no en el nomnbre del archivo. Git rastrea el contenido en lugar de los archivos