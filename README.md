# Laboratorio - Terminal básico

## Introducción
En este ejercicio vamos a simular que creas un proyecto desde cero, para ello te indicaremos el nombre
del proyecto, los ficheros a a adir y una serie de situaciones que tendrás que resolver.

Entregable: El entregable de esta documento es un fichero de texto en el que indicas la secuencia de
comandos que has empleado para completar el ejercicio y un enlace al repositorio creado en Github.

## Enunciado
Empezamos a trabajar en un proyecto en local desde cero.
### Arranque
Dentro de una carpeta vamos a añadir ficheros con documentación:
*principal.md*
```
# Principal
Este es el fichero principal
```

Nos damos cuenta de que es buena idea empezar a trabajar con Git, pero de momento no queremos
subir nada a la nube.
Pon aquí qué comando usarías para crear el repositorio en local:
```
git init
```

Queremos guardar lo que llevamos de proyecto (el fichero principal.md) en la base de datos de Git que
tenemos en local  Qu  comandos podemos ejecutar para hacer esto?
Nota(*) Si lo prefieres hacer en un comando también vale
```
git add .
git commit -m "Añadir principal.md y README.md"
```

### Ignorar
Resulta que la herramienta que usamos para editar ficheros va creando ficheros temporales con
extension .bak, vamos a simular esto, creamos dos ficheros nuevos:
*./detalle.md*
```
Esto es un texto de detalle
```

*./detalle.md.bak*
```
Esto es un texto de detal
```

Antes de subir a staging los cambios queremos ver en que estado están los ficheros, para ello
ejecutamos el comando:
```
git status
```

Anda! Queremos hacer commit del fichero detalle.md pero no queremos que se suban los ficheros con
extension .bak, así que decidimos a añdir una entrada al .gitignore. Qué contenido tendríamos que
añadir?
Indica aquí tu *.gitignore*
```
*.bak
```

Pista: para la extensión te va a hacer falta usar un patrón, más info:
https://www.atlassian.com/es/git/tutorials/saving-changes/gitignore

Ahora que lo tenemos vamos a meter los cambios en la base de datos de git (el fichero detalle.md). Qué
comandos o comando te harían falta?
Nota(*) Si lo prefieres hacer en un comando también vale
```
git add .
git commit -m "Añadir .gitignore, detalle.md y actualizar README.md"
```

### Subida a la nube
Toca subir esto a un repositorio en la nube, no queremos que se nos pierda el trabajo si se rompe nuestro
portatil.
Así que:
Crea un repositorio público en tu cuenta de Github, pon aquí el enlace al mismo:
https://github.com/pvvic/laboratorio-terminal-basico.git

Enlace tu local a ese servidor, pon aquí el comando:
```
git remote add origin https://github.com/pvvic/laboratorio-terminal-basico.git
````

Sube el contenido al servidor, pon aquí el comando:
```
git push https://g---PRIVADO---S@github.com/pvvic/laboratorio-terminal-basico.git
```