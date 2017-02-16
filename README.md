# Ejemplo de obtener 10 datos y compararlos

## Documentación
  * [función ctype_digit](http://php.net/manual/es/function.ctype-digit.php")
  * [función ctype_alpha](http://php.net/manual/es/function.ctype-alpha.php")
  * [función ctype_alnum](http://php.net/manual/es/function.ctype-alnum.php")
  
  Array que contiene los valores a comparar
```php
$datos = [ "1", "a", '2', "b", "3", "c", "4", "d", "5", "e2"]; 

for($i=0; $i<10; $i++){
    // la funcion ctype_digit() compara si solo hay numeros en la variable de entrada.
		if (ctype_digit($datos[$i])) { 
          // la funcion echo solo se imprime la varieble es un numero.
			echo $datos[$i]." Es un numero <br>"; 
		} 
    // la funcion ctyoe_alpha() revisa si solo hay letras en la variable de entrada.
		elseif(ctype_alpha($datos[$i])){ 
			echo $datos[$i]." contiene puras letras <br>";
		}
    // la funcion ctype_alnum() compara si los valores de la variable son alfanumericos
		elseif (ctype_alnum($datos[$i])) { 
			echo $datos[$i]." contiene caracteres alfanumericos <br>";	
		}
	}	
```
