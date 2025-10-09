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