# Ejemplo de obtener 10 datos y compararlos

## Documentación
  * [función ctype_digit](http://php.net/manual/es/function.ctype-digit.php")
  * [función ctype_alpha](http://php.net/manual/es/function.ctype-alpha.php")
  * [función ctype_alnum](http://php.net/manual/es/function.ctype-alnum.php")
   - - -
  
  Se declara un array con
```php
$datos = [ "1", "a", '2', "b", "3", "c", "4", "d", "5", "e2"];
```
- - -
Para hacerlo mas eficiente se iteran los datos a comparar. 

```php 
for($i=0; $i<10; $i++){
```
- - - 
Se usara la función `ctype_digit()` La cual compara los caracteres y regresa true si son puros numeros

```php
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
