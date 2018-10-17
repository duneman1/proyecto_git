# Proyecto Git #

Ejercicio para aprender a usar git

- Paso 1. Crear el repositorio

```shell
$ git init <nombre del proyecto>
```

- Paso 2. Crear el fichero .gitignore ( en nuestro caso ignorar node_modules)

```
node_modules/
```

- Paso 3. Crear el readme.md ( Se escribe en Markdown)

- Paso 4. Crear package.json ( El -y es para que no pida los datos y los rellene el automaticamente.)

```shell
$ npm init -y
```

- Paso 5. Mandar los ficheros inciales al amacenamiento temporal (El `.` es la abreviatura de `*.*`).

```shell
$ git add .
```

- Paso 6. Git status muestra el estado de los ficheros, en rojo si no estan añadidos al temporal y en verde pendiente del commit.

```shell
$ git status
```

- Paso 7. Realizamos un Commit -m es mensaje se pone entre comillas sencillas `''` si es powerShell y `""` si es cmd.

```shell
$ git commit -m 'Ficheros iniciales del proyecto'
```

- Paso 8. Cremos el origen del git (Seria la direccion de telefono).

```shell
$ git remote add origen https://github.com/duneman1/proyecto_git.git
```

- Paso 9. Ir a github a crear el repositorio, ya que no lo crea directamente con un push, pero por ejemplo gitLab si.

- Paso 10. Subimos el fichero master Github.

```shell
$ git push -u origin master
```
- Paso 11. Instalamos  las dependencias necesarias, como por ejemplo Bootstrap.

```shell
$ npm i bootstrap
```
- Paso 12. Git status muestra los ficheros modificados o untrack, .

```shell
$ git status
```

- Paso 13. Añadimos al temporal.

```shell
$ git add .
```

- Paso 14. Realizamos un commit.

```
$ git commit -m 'Instalación de Bootstrap'
```

- Paso 15. Vemos el log y no estamos sincronizados.

```shell
$ git log --oneline
```

- Paso 16. Sincronizamos con github

```shell
$ git push
```

- Paso 17. Vemos el log y el master y el origin estan en la misma linea, es que estan sicronizados en local y en github.

```shell
$ git log --oneline
```

- Paso 18. Creación de los ficheros web, html, css y JS.

- Paso 19. Añadimos a temporal los ficheros.

```shell
$ git add
```

- Paso 20. Creamos un commit.
 
```shell
 $ git commit -m 'Creación de ficheros WEB'
```

- Paso 21. Sincronizamos con github.

```shell
$ git push
```

- Paso 22. Vemos el log que todo este bien.

```shell
$ git log --oneline
```

- Paso 23. Nos movemos en el tiempo en el historial del git, al hacer el log los numeros hexagesimales que salen, es el punto de control(puntero), para movernos hay, se hace con checkout.

```shell
$ git checkout f241458
```

- Paso 24. Git nos avisa que tengamos cuidado que cualquier commit borraria los que estan por encima, asi que volvemos hacia atras, volviendo al ultimo commit.

```shell
$ git checkout master
```

- Paso 25. Creamos una nueva rama(alternativa) desde el commit que queremos en este caso es de cuando añadimos bootstrap.

```shell
$ git checkout f241458
$ git checkout -b alternativa
```

- Paso 26. Para moverse entre ramas es con checkout, master es la original y la rama es alternativa.

```shell
$ git checkout master
$ git checkout alternativa
```