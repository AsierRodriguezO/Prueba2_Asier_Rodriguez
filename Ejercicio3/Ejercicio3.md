# Ejercicio 3

## Crea una rama nueva llamada `Primera` y comprueba que existe.

> Para crear una rama nueva y comprobar que existe, puedes usar los siguientes comandos de Git:
```bash
git checkout -b Primera
git branch
```

## Crea un nuevo fichero en esta rama y fusiónalo con la principal.
> Para crear un nuevo fichero en la rama `Primera` y fusionarlo con la rama principal, puedes seguir estos pasos:
1. Asegúrate de estar en la rama `Primera`:
```bash
git checkout Primera
```


2. Crea un nuevo fichero, por ejemplo `fichero.txt`:
```bash
nano fichero.txt
```


3. Añade el fichero al área de preparación y haz un commit:
```bash
git add fichero.txt
git commit -m "Añadir fichero.txt en la rama Primera"
```


1. Cambia a la rama principal `main`:
```bash
git checkout main
```


5. Fusiona la rama `Primera` con la rama principal:
```bash
git merge Primera
```
## ¿Se ha producido algún conflicto al fusionar las ramas? 
> No, no se ha producido ningún conflicto al fusionar la rama `Primera` con la rama principal ya que solo se han realizado cambios en la nueva rama.

6. Borramos la rama `Primera`:
```bash     
git branch -d Primera
```     
Comprobamos que la rama `Primera` ha sido eliminada:
```bash
git branch
``` 

7. creamos una nueva rama llamada `Segunda` y repetimos el proceso anterior.
```bash
git checkout -b Segunda
nano conflicto.txt
git add conflicto.txt
git commit -m "Añadir conflicto.txt en la rama Segunda"
git checkout main
git merge Segunda
```
Modificamos el fichero `conflicto.txt` en la rama `main` para crear un conflicto:
```bash 
nano conflicto.txt
```
Añadimos y hacemos commit de los cambios en la rama `main`:
```bash 
git add conflicto.txt
git commit -m "Modificar conflicto.txt en la rama main"
git merge Segunda
```

hacemos una copia del conflicto para entrgarla

8. solucionamos el conflicto y hacemos un commit.
> Para solucionar el conflicto, abre el fichero `conflicto.txt` y busca las marcas de conflicto (`<<<<<<<`, `=======`, `>>>>>>>`). Edita el fichero para resolver el conflicto y luego guarda los cambios.
.