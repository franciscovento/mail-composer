
# Mail Composer

## Descripcion

Este proyecto usa pug para reutilizar componentes html que nos ayuden a mejorar la rápidez y precisión a la hora de maquetar emails. 


## Instalación de pug de forma global
```bash
  npm install -g pug-cli
```
Puedes ver la documentación aquí: https://pugjs.org/api/getting-started.html

#### Vscode:
- Pug beautify: Instala esta extensión en vscode para ayudar con el formateo. https://marketplace.visualstudio.com/items?itemName=mrmlnc.vscode-pugbeautify

### Correr el servidor
Para correr el servidor en modo watch escribir el siguiente comando dentro de la carpeta mail-composer
```bash
  pug -w . -o ./output  -P
```
Esto hará que cualquier modificación en los archivos que terminen en .pug los veas dentro de la carpeta "output". Dentro de esta carpeta entrarás el resultado html que finalmente copiarás en el servicio de correo electrónico.

Puedes utilizar live server dentro del archivo modificado en el output para ver los cambios en tiempo real. 


### Características principales

#### Mixins:
- Blocks: Son elementos que ocupan toda una fila. Generalmente agrupados bajo la etiqueta <tr>. Reciben parámetros para su reutilización dependiendo del contexto. 
- Components: Son elementos que ocupan una columna. Generalmente agrupados bajo la etiqueta <td>. También recibien parámetros para su reutilziación.
#### Templates:
- Secciones que no varian. (header, footer, legales, etc.)

#### Variables:
- Puedes crear variables a nivel de un componente o a nivel de página para utilizarlas durante el maquetado. Para más información ver documentación de Pug. 