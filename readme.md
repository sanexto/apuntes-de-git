# Curso Git desde cero
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos.

## Zonas de Git
1. Directorio de trabajo.
2. Area de preparacion.
3. Directorio Git.

## Flujo de trabajo basico en Git
1. Modificas una serie de archivos en tu directorio de trabajo.
2. Preparas los archivos, añadiéndolos a tu área de preparación.
3. Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

## Configurando Git por primera vez
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git config --global core.editor nano
git config --list
```

## Configuracion SSH en Windows
Usando Git Bash seguimos los siguientes pasos:

1. Creamos una carpeta donde almacenar las llaves para evitar problemas de rutas.

2. Ejecutamos el comando `ssh-keygen -t rsa -C "sanexto@gmail.com"`. El correo debe ser el mismo con el que nos registramos en Github para evitar posibles problemas. Dejamos el passphrase vacio y damos enter. Cuando nos pida la ruta escribimos la ruta que creamos en el paso 1.

3. Iniciamos ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"`.

4. Agregamos la llave ssh generada a ssh-agent ejecutando el comando `ssh-add`.

5. Desde ahora podemos hacer pull y push sin que GitHub no este pidiendo los datos de acceso.