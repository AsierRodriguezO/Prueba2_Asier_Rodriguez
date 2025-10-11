# Ejercicio 3

## Crea una rama nueva llamada `Primera` y comprueba que existe.

> Para crear una rama nueva y comprobar que existe, puedes usar los siguientes comandos de Git:
```bash
git branch Primera
git branch
```
![imagen](/Ejercicio3/imagenes/imagen.png)

## Crea un nuevo fichero en esta rama y fusiónalo con la principal.
> Para crear un nuevo fichero en la rama `Primera` y fusionarlo con la rama principal, puedes seguir estos pasos:
1. Asegúrate de estar en la rama `Primera`:
```bash
git checkout Primera
```
![imagen](/Ejercicio3/imagenes/imagen%20(1).png)

2. Crea un nuevo fichero, por ejemplo `fichero.txt`:
```bash
nano fichero.txt
```
![imagen](/Ejercicio3/imagenes/imagen%20(2).png)

3. Añade el fichero al área de preparación y haz un commit:
```bash
git add fichero.txt
git commit -m "Añadimos el primer fichero"
```
![imagen](/Ejercicio3/imagenes/imagen%20(3).png)

4. Cambia a la rama principal `master`:
```bash
git checkout master
```
![imagen](/Ejercicio3/imagenes/imagen%20(4).png)

5. Fusiona la rama `Primera` con la rama principal:
```bash
git merge Primera
```
![imagen](/Ejercicio3/imagenes/imagen%20(5).png)

## ¿Se ha producido algún conflicto al fusionar las ramas? 
> No, no se ha producido ningún conflicto al fusionar la rama `Primera` con la rama principal ya que solo se han realizado cambios en la nueva rama.

6. Borramos la rama `Primera` Comprobamos que la rama ha sido eliminada::
```bash     
git branch -d Primera
git branch
```
![imagen](/Ejercicio3/imagenes/imagen%20(6).png)

7. creamos una nueva rama llamada `Segunda` y repetimos el proceso anterior.
```bash
git branch Segunda
git checkout Segunda
```
![imagen](/Ejercicio3/imagenes/imagen%20(7).png)

```bash
nano conflicto.txt
git add conflicto.txt
git commit -m "Añadir conflicto.txt en la rama Segunda"
```
![imagen](/Ejercicio3/imagenes/imagen%20(8).png)

![imagen](/Ejercicio3/imagenes/imagen%20(9).png)

Modificamos el fichero `conflicto.txt` en la rama `main` para crear un conflicto:
```bash 
nano conflicto.txt
```
![imagen](/Ejercicio3/imagenes/imagen%20(10).png)

Añadimos y hacemos commit de los cambios en la rama `master`:
```bash 
git add conflicto.txt
git commit -m "Modificar conflicto.txt en la rama main"
```
![imagen](/Ejercicio3/imagenes/imagen%20(11).png)


Ahora hacemos el merge de la rama `Segunda` en `master`:
```bash 
git merge Segunda
```
![imagen](/Ejercicio3/imagenes/imagen%20(12).png)
hacemos una copia del conflicto para entrgarla

![imagen](/Ejercicio3/imagenes/imagen%20(13).png)

8. solucionamos el conflicto y hacemos un commit.

![imagen](/Ejercicio3/imagenes/imagen%20(14).png)

> Para solucionar el conflicto, abre el fichero `conflicto.txt` y busca las marcas de conflicto (`<<<<<<<`, `=======`, `>>>>>>>`). Edita el fichero para resolver el conflicto y luego guarda los cambios.
> 
![imagen](/Ejercicio3/imagenes/imagen%20(15).png)

Después de resolver el conflicto, añade el fichero al área de preparación y haz un commit:
```bash
git add conflicto.txt
git commit -m "Fichero arreglado"
```
![imagen](/Ejercicio3/imagenes/imagen%20(16).png)

Con esto, habrás solucionado el conflicto y hecho un commit con los cambios resueltos.