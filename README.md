# JavaScript 

[![aledc.com](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.com)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.com)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.com)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.com)




## Formatear un numero

Temenos el numero 460 millones que se vé así: 460000000, sin ninguna separación, entonces queremos lograr este resultado: 460.000.000

Esta función haciendo uso de __toString().Split()__  le dá el formato deseado.

```js
let ale =  460000000;

function numberWithCommas(x) {
    var parts = x.toString().split(".");
    parts[0] = parts[0].replace(/\B(?=(\d{3})+(?!\d))/g, ".");
    return parts.join(".");
}


numberWithCommas(ale);
````

Otra posibilidad de hacer esto mismo es haciendo uso de __toLocaleString__  . Esta función formatea el numero según el parámetro que se le pase, en este caso yo le paso __'en-US'__   
Si se deja en blanco, tomara el dato del navgador.   

```js
var n = 100000;
function numberWithCommas2(x) {

var ale2 = n.toLocaleString(
  'en-US', // dejar undefined sin coma, y usará el dato del browser
             // o indicar un string  'en-US' para usar un formato específico.
  { minimumFractionDigits: 2 }
);
return ale2;
}

numberWithCommas2(n);
````

