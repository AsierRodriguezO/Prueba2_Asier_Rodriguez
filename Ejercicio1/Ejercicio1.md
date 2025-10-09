# ACTIVIDAD1

### Repositorio local en Windows 
> Creamos un nuevo repositorio local en Git llamado Prueba2_Asier_Rodríguez.

![alt text](/Ejercicio1/Imagenes/imagen.png)

>Ahora vamos a hacer un **`git init`** en la carpeta creada para hacerlo un repositorio local.

![alt text](/Ejercicio1/Imagenes/imagen%20(1).png)

>Creamos 2 archivos de texto plano en la carpeta del repositorio local.
>
![alt text](/Ejercicio1/Imagenes/imagen%20(2).png)

>En este momento toca hacer un **`git add .`** para añadir los archivos al área de preparación.
>Con **`git status`** podemos ver el estado del repositorio en todo momneto y tambien puedes apreciar los estados de los archivos.

![alt text](/Ejercicio1/Imagenes/imagen%20(3).png)

![alt text](/Ejercicio1/Imagenes/imagen%20(4).png)

## Repositorio remoto en GitHub
>Ya que necesitamos conectarnos a un repositorio remoto, creamos uno en GitHub llamado Prueba2_Asier_Rodríguez.Este repositorio tiene que estar vacio.

![alt text](/Ejercicio1/Imagenes/imagen%20(5).png)

>Despues de eso nos conectamos al repositorio remoto con el comando **`git remote add origin URL-DEL-REPOSITORIO`**.
>Pero como queremos permisos tenemos que poner el usuario y la clave en mitada del comando.

![alt text](/Ejercicio1/Imagenes/imagen%20(6).png)

>Subimos el repositorio local al remoto con el comando **`git commit -m "Texto que quieras poner"`** y **`git push -u origin main`**.
>Comprobamos que el repositorio remoto tiene los archivos subidos.

![alt text](/Ejercicio1/Imagenes/imagen%20(7).png)

![alt text](/Ejercicio1/Imagenes/imagen%20(8).png)

## Debian

![alt text](/Ejercicio1/Imagenes/imagen%20(9).png)

>Como en apartados anteriores creamos un repositorio local en Debian llamado Prueba2_Asier_Rodríguez.
>Hacemos un **`git init`** en la carpeta creada para hacerlo un repositorio local.

![alt text](/Ejercicio1/Imagenes/imagen%20(10).png)

>Una vez realizado el repositorio local, nos descargamos el repositorio remoto que hemos creado en GitHub con el comando **`git clone URL-DEL-REPOSITORIO`**.
>Al igual que en el otro ejercicio si queremos permisos tenemos que poner el usuario y la clave en mitada del comando.

![alt text](/Ejercicio1/Imagenes/imagen%20(11).png)

>Toca comprobar que el repositorio remoto tiene los archivos subidos.

![alt text](/Ejercicio1/Imagenes/imagen%20(12).png)

## Modificaciones
>Vamos a el repositorio en windows y modificamos un archivo de texto plano y añadimos otro archivo de texto plano.
>Despues subimos los cambios al repositorio remoto como ya hemos hecho antes.

![alt text](/Ejercicio1/Imagenes/imagen%20(13).png)
![alt text](/Ejercicio1/Imagenes/imagen%20(14).png)

>Por ultimo nos vamos al repositorio en Debian y hacemos un **`git pull`** para descargar los cambios del repositorio remoto.

![alt text](/Ejercicio1/Imagenes/imagen%20(15).png)
