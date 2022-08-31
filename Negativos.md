# Representación de numeros negativos en binario

Para representar numeros binarios en negativo existen distintos métodos para representar la negatividad en binario, entre algunas tenemos:

- Signo y Magnitud
- Complemento a 1
- Complemento a 2
- Mecanismo de exceso


#### Signo y Magnitud

Para este método se utiliza un rango de 16 bits para representar binarios.

Ej.:  

$-255$

  - Se toma el numero como si fuese positivo:
    - $255$ $\rightarrow$ $0$ $0000000$ $11111111$
  - Luego el bit más significativo toma el valor del signo: 1 para **negativo** y 0 para **positivo**
    - $255$ $\rightarrow$  **$1$** $0000000$ $11111111$    

Ejemplos:

- $256$  $\rightarrow$ $0$ $0000001$ $00000000$
- $520$  $\rightarrow$ $0$ $0000010$ $00001000$
- $-355$ $\rightarrow$ $1$ $0000001$ $00111000$

#### Complemento 1

Para este metodo se trabaja como si el numero fuese positivo, se convierte en binario y a este resultado se le invierten los valores.

Ej.:  

$-362$
  - Se trabaja el binario como positivo
    - $362$ $\rightarrow$ $0$ $0000001$ $01101010$
  - Ahora se invierten todos los valores del binario y se añade el signo
    - $-362$ $\rightarrow$ $0$ $0000001$ $01101010$ $\rightarrow$ $1$ $1111110$ $10010101$