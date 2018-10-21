# git tag
Lista las etiquetas existentes.

## git tag nombre-etiqueta
Lista las etiquetas en orden alfabetico.

## git tag -a nombre-etiqueta -m 'mensaje de la etiqueta'
Etiqueta anotada. Se guarda en la base de datos de Git como un objeto entero. Tiene un checksum; contiene el nombre del etiquetador, correo electrónico y fecha; y tiene un mensaje asociado.

```
git tag -l 'v1.*'
```
Lista las etiquetas que coincidan con el patron especificado.
