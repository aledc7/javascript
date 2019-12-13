# JavaScript 

[![aledc.tk](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.tk)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.tk)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.tk)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.tk)


# Recalcular dos input

Este ejemplo recalcula automaticamente el valor de dos input dinamicamente para que la suma siempre sea 100.   
En caso de que se cambie el valor de alguno de los input, el otro se reajustará automáticamente. 

```php
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
    <title>Recalcula Input</title>

    <script>
      $(document).ready(function(){
          
        # Logica para el primer input
        $('input[name="text1"]').prop('readonly', false).blur(function(){
        $('input[name="text2"]').val(100 - $('input[name="text1"]').val() );
        });
        
        # Logica para el segundo input
        $('input[name="text2"]').prop('readonly', false).blur(function(){
        $('input[name="text1"]').val(100 - $('input[name="text2"]').val() );
        });
    });
    </script>
    
    
    
  </head>
  <body>
    <p>El total de estos dos input sumará 100, si se cambia algun numero, se ajusta automaticamente</p>

        <input type="text" name="text1" size="5"> Valor 1<br />
        <input type="text" name="text2" size="5"> Valor 2<br />
        

  </body>
</html>
````

