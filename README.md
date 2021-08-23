# color-flipper [![GitHub license](https://img.shields.io/github/license/larrykevin/color-flipper)](https://github.com/larrykevin/color-flipper/blob/master/LICENSE)

Generador de colores aleatorios con javascript

![colorflipper__demo](http://g.recordit.co/qyoQJ5Inmr.gif)

## 🚀 Instalación
1. Utiliza el comando `git clone` para clonar el proyecto
2. Accede a la carpeta del proyecto `cd color-flipper`
3. Abre el proyecto desde editor de código. Puedes descargar el plugin `Five Server` en Visual Studio Code para correr el proyecto.

## 🍩 Contenido　
Ingresando a la pestaña de HEX observarás la aplicación principal.

### En hex.js
```javascript
// Establecemos variables seleccionando etiquetas del DOM
const hex = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, "A", "B", "C", "D", "E", "F"];
const btn = document.getElementById('btn');
const color = document.querySelector('.color');

// Luego creamos un evento click para el botón
btn.addEventListener('click', function() {
    let hexColor = '#';
    for (let i = 0; i < 6; i++) {
        hexColor += hex[getRandomNumber()];
    }
    color.textContent = hexColor;
    document.body.style.backgroundColor = hexColor;
})

// Creamos una función para obtener un número aleatorio de la longitud de nuestro array
function getRandomNumber() {
    return Math.floor(Math.random() * hex.length);
}
```
## 🔓 License
The MIT License (MIT)