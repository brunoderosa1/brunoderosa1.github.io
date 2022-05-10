# pdf-viewer

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

----------------------------------------------------------------------------

## Desarrollo de desafío Vue.js


Se solicita crear una aplicación usando Vue.js que permita visualizar un documento PDF en una ventana que se sobreponga.

Para resolver el problema pensé en dos caminos, utilizar la API de Adobe o utilizar el lector de PDF nativo del dispositivo. 

Si uso la API de Adobe para manipular documentos, necesito adquirir una key que va a estar vinculada a un dominio en particular, pero ganaría independencia de las condiciones iniciales del equipamiento del usuario por lo que la solución limitaría su aplicabilidad a que el usuario tenga un navegador compatible con la tecnología.

Por otro lado, si uso el lector de PDF nativo del sistema del usuario, dependo de una condición externa que no puedo controlar, pero en contrapartida prácticamente todos los dispositivos que tienen acceso a internet cuentan con un lector de PDF incorporado.

Particularmente considero que la solución más apropiada al problema es usar el lector nativo del dispositivo del usuario ya que el objetivo de esta tarea es poder visualizar un documento PDF y de esta manera el objetivo se cumple sin tener que utilizar una API que tiene que cargar, ejecutarse y ser utilizable por el usuario mientras que el lector nativo del dispositivo es el software al que está familiarizado el usuario por lo que no debería presentar barreras en su uso.

