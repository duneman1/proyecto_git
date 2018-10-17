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

```
$ git commit -m 'Ficheros iniciales del poryecto'
```

- Paso 8. Cremos el origen del git (Seria la direccion de telefono).

$