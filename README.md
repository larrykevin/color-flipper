# color-flipper [![GitHub license](https://img.shields.io/github/license/larrykevin/color-flipper)](https://github.com/larrykevin/color-flipper/blob/master/LICENSE)

Generador de colores aleatorios con javascript

![colorflipper__demo](http://g.recordit.co/qyoQJ5Inmr.gif)

## 馃殌 Instalaci贸n
1. Utiliza el comando `git clone` para clonar el proyecto
2. Accede a la carpeta del proyecto `cd color-flipper`
3. Abre el proyecto desde editor de c贸digo. Puedes descargar el plugin `Five Server` en Visual Studio Code para correr el proyecto.

## 馃崺 Contenido銆?
Ingresando a la pesta帽a de HEX observar谩s la aplicaci贸n principal.

### En hex.js
```javascript
// Establecemos variables seleccionando etiquetas del DOM
const hex = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, "A", "B", "C", "D", "E", "F"];
const btn = document.getElementById('btn');
const color = document.querySelector('.color');

// Luego creamos un evento click para el bot贸n
btn.addEventListener('click', function() {
    let hexColor = '#';
    for (let i = 0; i < 6; i++) {
        hexColor += hex[getRandomNumber()];
    }
    color.textContent = hexColor;
    document.body.style.backgroundColor = hexColor;
})

// Creamos una funci贸n para obtener un n煤mero aleatorio de la longitud de nuestro array
function getRandomNumber() {
    return Math.floor(Math.random() * hex.length);
}
```
## 馃敁 License
The MIT License (MIT)