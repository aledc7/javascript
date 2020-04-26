# JavaScript 

[![aledc.tk](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.tk)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.tk)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.tk)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.tk)




## Deshabilitar un boton y ejecutar una funcion luego de X lapso de tiempo.   

```js

function disable_button(){

      // deshabilito boton enviar  
      $('#enviar').prop('disabled', true);
      
      // Ejecutar la funcion ale2()luego de 4 segundos
      window.setTimeout( ale2, 4000 ); // 4 segundos
      }
      
      
// Otra manera de poner un delay:

// Envuelvo mi funcion o evento dentro de un setTimeout, y luego le pongo el tiempo en milisegundos (1000 = 1 seg.)
setTimeout(function() {
          alert("Algo");
            }, 4000);
      
      
      
````

# Mostrar un Objeto en un alert o en un colsole.log
```php
// Antepongo JSON.Stringify
alert(JSON.stringify(miobjeto));

// Lo mismo en los console.log
console.log(JSON.stringify(miobjeto));
````





