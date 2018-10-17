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

```
$ git status
```
