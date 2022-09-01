# Punto Flotante

Para representar numeros decimales en binario existen 2 estandar para estos mismo, estos son:
- **IEEE 754 Presición Simple (32 bits)**
  - Su composicion es de:
    - 1 bit para el signo
    - 8 bits para el exponente
    - 23 bits para la mantisa
- **IEEE 754 Doble Presición (64 bits)**
    - Su composicion es de:
      - 1 bit para el signo
      - 11 bits para el exponente
      - 52 bits para la mantisa

Ej.: 

Utilizando el estandar IEEE 754 de 32 bits, represente el valor decimal **47.9**

Paso 1: Convertir la parte entera a binaria:
- $47 \rightarrow 101111$

Paso 2: Convertir la parte decimal a binario de la siguiente forma:
- Se toma el valor decimal: 0.9 y se multplica por 2 hasta que no existan mas decimales en su resultado, si a este valor entrega un decimal con parte entera, esta se extrae para el binario y se trabaja con la parte decimal:
  - $0.9 * 2 = 1.8 \rightarrow 1$
  - $0.8 * 2 = 1.6 \rightarrow 1$
  - $0.6 * 2 = 1.2 \rightarrow 1$
  - $0.2 * 2 = 0.4 \rightarrow 0$
  - $0.4 * 2 = 0.8 \rightarrow 0$
  - $0.8 * 2 = 1.6 \rightarrow 1$
- Como nos damos cuenta, al momento de multplicar y llegar al 0.8 en este caso de manera ciclica, estos binarios se repiten, quedando de la siguiente manera:
- $0.9 \rightarrow .11100110011001100$

Quedando el numero: 101111.1110011001100

Luego, se corre el **.** hasta la posicion entera:

$1.011111110011001100 * 2^5$

Con esto tenemos la mantisa.

Luego el exponente se calcula como el exceso más el exponente anterior:

$127 + 5 = 132$

Luego, en el binario del exponente, se rellena con este número

Exponente $\rightarrow 10000100$

Finalmente se compone el numero completo:

Signo / Exponente / Mantisa Hasta completar los 23 bits

$0$ $10000100$ $01111111001100110011001$

Y con esto tenemos el binario expresado en decimal.


Ejercicios:

- Convertir:
  - $126.23$
  - $59.6$
  - $-176.25$
  - $86.5$
  - $-128.75$
