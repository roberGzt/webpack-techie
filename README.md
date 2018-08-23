# Webpack Techie #

## ¿Qué es? ##
[Webpack](https://webpack.js.org) es una herramienta para generar builds de aplicaciones webs. Una vez configurada, escanea el proyecto buscando dependencias entre distintos modulos y arma **bundles** o paquetes con todos los archivos cargados en el orden correcto.

## ¿Para qué sirve? ##
Además de generar bundles con los distintos archivos que se necesitan en nuestra aplicación web. Webpack nos permite transformar de otras formas nuestro código fuente.

Mediante el uso de **loaders** podemos procesar archivos de distintos tipos y aplicarles transformaciones, como por ejemplo compilar:
* scss a css.
* typescript a javascript.
* convertir ES6 a ES5. compatible con browsers antiguos.

Además de loaders, que procesan archivos de tipos particulares generando finalmente bundles, existen los llamados **plugins** que son componentes que nos permiten realizar procesamientos sobre los bundles generados.

## ¿Cómo se instala? ##
#### Prerequisitos ####
* [Node.js](https://nodejs.org/es/)

Luego de tener instalado node.js, dentro de la carpeta del proyecto en el que queremos usar webpack debemos inicializar npm para que gestione nuestras dependencias sobre librerias (entre ellas, webpack):
```
npm init -y
```

Usamos la opción *-y* para aceptar las opciones por defecto.
Esto nos creará un archivo **package.json** en nuestro proyecto.

Con el package.json creado en nuestro proyecto ya podemos instalar webpack:

```
npm install webpack webpack-cli --save-dev
```