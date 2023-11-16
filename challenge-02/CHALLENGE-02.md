<h1>** Mini Compiler Challenge **</h1>
<p>En el mundo del espionaje, se utiliza un lenguaje de codificación con símbolos que realizan operaciones matemáticas simples.</p>
<p>Tu tarea es crear un mini compilador que interprete y ejecute programas escritos en este lenguaje de símbolos.</p>

Las operaciones del lenguaje son las siguientes:
<ul>
  <li>"#" Incrementa el valor numérico en 1.</li>
  <li>"@" Decrementa el valor numérico en 1.</li>
  <li>"*" Multiplica el valor numérico por sí mismo.</li>
  <li>"&" Imprime el valor numérico actual.</li>
</ul>
<p>El valor numérico inicial es 0 y las operaciones deben aplicarse en elorden en que aparecen en la cadena de símbolos.</p>

  <h2>Ejemplos de entrada:</h2>
<pre>
Entrada: "##*&"
Salida esperada: "4"
Explicación: Incrementa (1), incrementa (2), multiplica (4), imprime (4).

Entrada: "&##&*&@&"
Salida esperada: "0243"
Explicación: Imprime (0), incrementa (1), incrementa (2), imprime (2), multiplica (4), imprime (4), decrementa (3), imprime (3).
</pre>

** Tu desafío: **
Desarrolla un mini compilador que tome una cadena de texto y devuelva otra cadena de texto con el resultado de ejecutar el programa.

** Cómo resolverlo **
1. Resuelve el mensaje que encontrarás en este archivo: https://codember.dev/data/message_02.txt

2. Crea un programa al que le pases como entrada el mensaje anterior. Envía la salida con el comando "submit" en la terminal, por ejemplo así:
submit 024899488