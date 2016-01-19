# Static website starter project #

## Tecnologie utilizzate ##

- Scaffolding:
    - [Bower](http://bower.io)
    - [Grunt](http://gruntjs.com/)

- Javascript 
    - [ES5 Shim](https://github.com/es-shims/es5-shim)
    - [Modernizr](http://modernizr.com)
    - [jQuery](https://jquery.com) (v1.12)

- CSS3 
    - [SASS](http://sass-lang.com) with
        - ([Bourbon](http://bourbon.io) 
        - [Neat](http://neat.bourbon.io))

## Struttura directory ##

La struttura riportata mostra solamente i file necessari allo sviluppo/rilascio del sito.

Alcune directory potrebbero comparire dopo la prima ```build``` del progetto.

```
root
+-- src -> directory sviluppo
|   +-- images
|   +-- scripts
|   |   +-- main.js
|   +-- styles
|   |   +-- fonts
|   |   +-- _mixins.scss
|   |   +-- _variables.scss
|   |   +-- main.scss
|   +-- index.html
|   +-- apple-touch-icon.png
|   +-- favicon.ico
|   +-- robots.txt
|   +-- sitemap.xml
+-- dist -> dirctory output build progetto
+-- Gruntfile.js -> configurazione task Grunt
+-- bower.json -> elenco dipendenze del sito
+-- package.json -> elenco dipendeze del progetto
```

## Setup ##

Installare [Node.js](https://nodejs.org/), aprire una finestra del terminale, spostarsi nella directory del progetto ed eseguire i seguenti comandi: 

```
npm install -g grunt-cli
npm install -g bower
npm install
``` 

## Workflow ##

### Sviluppo ###

- Aprire una finestra del terminale e spostarsi nella directory del progetto

- Eseguire il comando `grunt serve`

- Verrà  aperta una finestra del browser con auto refresh all'indirizzo ```localhost:3000```

- Al salvataggio di qualunque file verrà  automaticamente fatto un build del progetto e ricaricata la pagina sul browser

### Test rilascio ###

- Aprire una finestra del terminale e spostarsi nella directory del progetto

- Eseguire il comando `grunt serve:dist`

- Verrà aperta una finestra del browser con la versione minificata del sito all'indirizzo ```localhost:9000```


### Rilascio ###

- Aprire una finestra del terminale e spostarsi nella directory del progetto

- Eseguire il comando `grunt build`

- Copiare il contenuto della directory `dist` sul server di produzione tramite un client FTP

## Editor consigliati ##

- [Sublime Text](http://www.sublimetext.com/3)

- [Atom](https://atom.io/)

## Credits ##

[Gabriele Destefanis](http://destefanis.eu) @ [Top Solution](http://topsolution.it) <g.destefanis@topsolution.it>
