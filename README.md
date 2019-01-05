# STR-util
Implementation of Split and Join functions  in C

Split:
Devuelve en un arreglo dinámico terminado en NULL con todos los subsegmentos
de ‘str’ separados por el carácter ‘sep’. Tanto el arreglo devuelto como las
cadenas que contiene son allocadas dinámicamente.
Quien llama a la función toma responsabilidad de la memoria dinámica del
arreglo devuelto. La función devuelve NULL si falló alguna llamada a
malloc(), o si ‘sep’ es '\0'.

Para liberar el arreglo dinamico de cadenas creado mediante split se utiliza la funcion free_strv, la cual recibe el arreglo dinamico.


Join:
Devuelve una cadena, allocada dinámicamente, resultado de unir todas las
cadenas del arreglo terminado en NULL ‘strv’.
Quien llama a la función toma responsabilidad de la memoria dinámica de la
cadena devuelta. La función devuelve NULL si no se pudo allocar memoria.
