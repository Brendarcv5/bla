# Observatorio


> Observatorio UdeG [Angular 2](https://angular.io)
 ([Router](https://angular.io/docs/js/latest/api/router/), [Forms](https://angular.io/docs/js/latest/api/forms/),
[Http](https://angular.io/docs/js/latest/api/http/),
 [TypeScript](http://www.typescriptlang.org/),
  [@types](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=0ahUKEwjgjdrR7u_NAhUQ7GMKHXgpC4EQFggnMAI&url=https%3A%2F%2Fwww.npmjs.com%2F~types&usg=AFQjCNG2PFhwEo88JKo12mrw_4d0w1oNiA&sig2=N69zbO0yN8ET7v4KVCUOKA), 
  [TsLint](http://palantir.github.io/tslint/), 
   y [Webpack 2](http://webpack.github.io/) by [Flatlogic](https://flatlogic.com).
  

### Quick start
**Asegúrese de tener la versión de Node  >= 5.0 y NPM >= 3**

En caso de no tener Node, descargar de [Node Js](https://nodejs.org/es/download/) 

Versión Recomenda: Node.js  `v6.11.0` *LTS*  *(con **npm** `3.10.10` incluido)*, para 	el correcto funcionamiento.

>**Instalación**
	> - *Ejecutar* ` node-v6.11.0-x64.msi`

```bash
# cambiar de directorio a nuestro repo 
cd observatorio-front

# instalar el repo con npm
npm install

# iniciar el servidor
npm start

```
Ir [http://0.0.0.0:3000](http://0.0.0.0:3000) ó [http://localhost:3000](http://localhost:3000) en el navegador.

# Tabla de Contenido
* [Estructura del Archivo](#file-structure)
* [Comenzando](#getting-started)
    * [Dependencias](#dependencies)
    * [Instalación](#installing)
    * [Ejecutando la app](#running-the-app)
* [Configuración](#configuration)



## Estructura del Archivo


```
observatorio/
 ├──config/                    * our configuration
 |   ├──helpers.js             * helper functions for our configuration files
 │   ├──webpack.dev.js         * our development webpack config
 │   ├──webpack.prod.js        * our production webpack config
 │
 ├──src/                       * our source files that will be compiled to javascript
 |   ├──main.browser.ts        * our entry file for our browser environment
 │   │
 |   ├──index.html             * Index.html: where we generate our index page
 │   │
 |   ├──polyfills.ts           * our polyfills file
 │   │
 |   ├──vendor.ts              * our vendor file
 │   │
 │   ├──app/                   * WebApp: folder
 │   │   └──app.ts             * App.ts: a simple version of our App component components
 │   │
 │   └──assets/                * static assets are served here
 │       ├──icon/              * our list of icons from www.favicon-generator.org
 │       ├──robots.txt         * for search engines to crawl your website
 │       └──humans.txt          * for humans to know who the developers are
 │
 │
 ├──tslint.json                * typescript lint config
 ├──typedoc.json               * typescript documentation generator
 ├──tsconfig.json              * config that webpack uses for typescript
 ├──package.json               * what npm uses to manage it's dependencies
 └──webpack.config.js          * webpack main configuration file

```

# Comenzando
## Dependencias
Lo que se necesita para ejecutar está app:
* `node` y `npm`
* Asegúrese de que está ejecutando la última versione de Node `v4.x.x`+ (or `v5.x.x`) y NPM `3.x.x`+
>Si tiene `nvm` instalado, lo que es muy recomendable (` brew install nvm`) puede hacer un `nvm install --lts && nvm use` en `$` para ejecutar el último Node LTS.
 

## Instalación
* `npm install` para instalar todas las dependencias.
* `npm start` para iniciar el servidor. 

### Servidor
```bash
# development
npm start
# production
npm run build:prod
npm run server:prod
```

## Otros Comandos

### Crear Archivos
```bash
# development
npm run build:dev
# production
npm run build:prod
```


### Ver y Crear Archivos
```bash
npm run watch
```

# Configuración
Los archivos de configuración se están en `config/`. Actualmente estamos usando webpack.

