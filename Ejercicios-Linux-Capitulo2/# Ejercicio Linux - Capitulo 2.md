# # Ejercicio Linux - Capitulo 2

[TOC]

## Comandos Utilizados

![image-20250924101509461](C:\Users\2dawd26\AppData\Roaming\Typora\typora-user-images\image-20250924101509461.png)

## Ejercicios Prácticos

1. ¿En qué directorio se encuentran los ficheros de configuración del sistema?

​	Los ficheros de la configuración del sistema se encuentran en el directorio /etc

2. Para entrar en un sistema Linux hace falta a) nombre de usuario, contraseña y dirección IP, b) nombre de usuario y contraseña o c) únicamente una contraseña..

   Nombre de usuario y contraseña

3. Muestra el contenido del directorio actual. 

   

   ```
   $ ls
   ```

   <img src="C:\Users\2dawd26\AppData\Roaming\Typora\typora-user-images\image-20250924104523081.png" alt="image-20250924104523081" style="zoom: 50%;" />

4. Muestra el contenido del directorio que está justo a un nivel superior

   ![image-20250924111635739](C:\Users\2dawd26\AppData\Roaming\Typora\typora-user-images\image-20250924111635739.png)

6. ¿En qué día de la semana naciste?, utiliza la instrucción cal para averiguarlo

   ```
   $ cal 9 2006
   ```

   ![image-20250924111002056](C:\Users\2dawd26\AppData\Roaming\Typora\typora-user-images\image-20250924111002056.png)
   
   6. Muestra los archivos del directorio /bin
   
   ```
   $ ls /bin
   ```
   
   ![image-20250926104020552](./# Ejercicio Linux - Capitulo 2.assets/image-20250926104020552.png)

7. Suponiendo que te encuentras en tu directorio personal (/home/nombre), muestra un listado del contenido de /usr/bin a) con una sola línea de comando, b) moviéndote paso a paso por los directorios y c) con dos líneas de comandos.

a) 

```
$ ls /usr/bin
```

![image-20250926105734726](./# Ejercicio Linux - Capitulo 2.assets/image-20250926105734726.png)

b)

```
$ cd/
$ cd usr     
$ cd bin     
$ ls 
```

![image-20250926105906494](./# Ejercicio Linux - Capitulo 2.assets/image-20250926105906494.png)

c)

```
$ cd /usr/bin
$ls
```

![image-20250926110119405](./# Ejercicio Linux - Capitulo 2.assets/image-20250926110119405.png)

8. Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando).

```
$ ls -R / etc
```

![image-20250926110749976](./# Ejercicio Linux - Capitulo 2.assets/image-20250926110749976.png)

9. Muestra todos los archivos del directorio /usr/X11R6/bin ordenados por tamaño (de mayor a menor). Sólo debe aparecer el nombre de cada fichero, sin ninguna otra información adicional.

```
$ ls -S /usr/X11R6/bin
```

![image-20250926111225461](./# Ejercicio Linux - Capitulo 2.assets/image-20250926111225461.png)

10.  Muestra todos los archivos del directorio /etc ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

    ```
    $ ls -lhS /etc
    ```

    ![image-20250926111459538](./# Ejercicio Linux - Capitulo 2.assets/image-20250926111459538.png)

11.  Muestra todos los archivos del directorio /bin ordenados por tamaño (de menor a mayor). Sólo debe aparecer el tamaño y el nombre de cada fichero, sin ninguna otra información adicional. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

    ```
    $ ls -lhS /bin
    ```

    ![image-20250926111615546](./# Ejercicio Linux - Capitulo 2.assets/image-20250926111615546.png)

    12.Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta absoluta.

    ```
    $ ls /
    ```

    ![image-20250926111806518](./# Ejercicio Linux - Capitulo 2.assets/image-20250926111806518.png)

13. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta relativa. Suponemos que el directorio actual es /home/elena/documentos.

    ```
    $ ls ../../..
    ```

    ![image-20250926121101721](./# Ejercicio Linux - Capitulo 2.assets/image-20250926121101721.png)

14. Crea el directorio gastos dentro del directorio personal.

    ```
    $ mkdir ~/gastos
    ```

    ![image-20250926121913596](./# Ejercicio Linux - Capitulo 2.assets/image-20250926121913596.png)

15. ¿Qué sucede si se intenta crear un directorio dentro de /etc?

    ```
    $ mkdir /etc/nuevo_directorio
    ```

    Para que funcione necesitamos permisos de administrador y para eso escribiríamos sudo delante del mkdir 

![image-20250926122102293](./# Ejercicio Linux - Capitulo 2.assets/image-20250926122102293.png)

16 .Muestra el contenido del fichero /etc/fstab

```
$ cat /etc/fstab
```

![image-20250926122532473](./# Ejercicio Linux - Capitulo 2.assets/image-20250926122532473.png)

17. Muestra las 10 primeras líneas del fichero /etc/bash.bashrc

    ```
    $ head /etc/bash.bashrc
    ```

    ![image-20250926122845864](./# Ejercicio Linux - Capitulo 2.assets/image-20250926122845864.png)

18. Crea la siguiente estructura de directorios dentro del directorio de trabajo personal:

    ```
    $ mkdir trabajoPersonal
    $ cd trabajoPersonal
    $ mkdir multimedia
    $ cd multimedia
    $ mkdir musica
    $ mkdir imagenes
    $ mkdir video
    $ mkdir presentaciones
    $ cd imagenes
    $ mkdir personales
    $ mkdir otras
    ```

    ![image-20251001111338090](./# Ejercicio Linux - Capitulo 2.assets/image-20251001111338090.png)

    ![image-20251001111433901](./# Ejercicio Linux - Capitulo 2.assets/image-20251001111433901.png)

    

## Ejercicios Prácticos Comandos

1. Crea un archivo prueba.txt y dale permisos rw-r----- usando modo simbólico.

   ```
   $ touch prueba.txt
   $ chmod u=rw,g=r,o= prueba.txt
   ```

   ![image-20251001100809316](./# Ejercicio Linux - Capitulo 2.assets/image-20251001100809316.png)

![image-20251001100834971](./# Ejercicio Linux - Capitulo 2.assets/image-20251001100834971.png)

2. Haz que solo el grupo pueda escribir en notas.txt .

   ```
   $ touch notas.txt
   $ chmod g+w,u-w,o-w notas.txt
   ```

   ![image-20251001101754790](./# Ejercicio Linux - Capitulo 2.assets/image-20251001101754790.png)

![image-20251001101817322](./# Ejercicio Linux - Capitulo 2.assets/image-20251001101817322.png)

3. Cambia el propietario de tarea.doc a ana y el grupo a profes .

```
$ sudo adduser ana
$ sudo groupadd profes
$ touch tarea.doc
$ sudo chown ana:profes tarea.doc
```

![image-20251001102845168](./# Ejercicio Linux - Capitulo 2.assets/image-20251001102845168.png)

![image-20251001102917709](./# Ejercicio Linux - Capitulo 2.assets/image-20251001102917709.png)

4. Quita todos los permisos a otros sobre config.cfg

   ```
   $ chmod o-rwx config.cfg
   ```

   ![image-20251001104124854](./# Ejercicio Linux - Capitulo 2.assets/image-20251001104124854.png)

5. Pon rwx a todos en un script llamado run.sh .

   ```
   $ touch run.sh
   $ chmod 777 run.sh
   ```

   ![image-20251001104816396](./# Ejercicio Linux - Capitulo 2.assets/image-20251001104816396.png)