# Ejercicios

#### Indique de acuerdo al estándar IEEE 754 de 32 bits el valor binario del siguiente número fraccionario (1.93)
    **-94,475**

    Escriba su resultado en una sola secuencia binaria de 32 bits

Signo: 1

Exponente: 10000101

Mantisa: 01111001111001100110011

#### Solucion:

Parte entera:
 - $94 \rightarrow 01011110$
 - $64 + 16 + 8 + 4 + 2$
 - $0 + 64 + 0 + 16 + 8 + 4 + 2 + 0$
 - $0 1 0 1 1 1 1 0$

Parte Decimal:
 - $0.475 * 2 = 0.95 \rightarrow 0$
 - $0.95 * 2 = 1.9 \rightarrow 1$
 - $0.9 * 2 = 1.8 \rightarrow 1$
 - $0.8 * 2 = 1.6 \rightarrow 1$
 - $0.6 * 2 = 1.2 \rightarrow 1$
 - $0.2 * 2 = 0.4 \rightarrow 0$
 - $0.4 * 2 = 0.8 \rightarrow 0$
 - $0.8 * 2 = 1.6 \rightarrow 1$
 - $0.6 * 2 = 1.2 \rightarrow 1$

Y como se puede notar, existe el ciclo: **$0011$**

Mantisa y expontente:
 1. Parte Entera + Parte Decimal
    1. $01011110.0111100110011$
 2. Se corre la coma hasta el ultimo 1, y se añade el exponente
    1. $1.0111100111100110011 * 2^6$
 3. Se sigue completando la mantisa con el ciclo hasta los 23 bits
    1. $01111001111001100110011$
 4. Se Calcula el valor binario del exponente utilizando el Mecanismo de Exceso
    1. $127 + 6 = 133 \rightarrow 128 + 4 + 1 \rightarrow 10000101$
 5. Finalmente se juntan todas las partes: Signo Exponente Mantisa

Resultado: $1 10000101 01111001111001100110011$

<br><br>

#### Cual es el valor Binario del siguiente valor Hexadecimal (3.5)

    75

#### Solución 1:

 1. Convertir los digitos independientes a binario usando 4 bits.
    1. $7 \rightarrow 4 + 2 + 1 \rightarrow 0111$
    2. $5 \rightarrow 4 + 1 \rightarrow 0101$
    3. Se juntan los digitos: $01110101$

#### Solución 2:
 1. Covertir el digito a decimal:
    1. $7 * 16^1 + 5 * 16^0$
    2. $7 * 16 + 5 * 1$
    3. $112 + 5$
    4. $117$
 2. Convertir el decimal a binario:
    1. $117$
    2. $64 + 32 + 16 + 4 + 1$
    3. $01110101$

  - [ ] a) 111001
  - [ ] b) 1111111
  - [ ] c) 1110111
  - [X] d) 1110101

<br><br>

#### Cual es la equivalencia Hexadecimal del siguiente valor decimal (4.0)

    58

#### Solución:

  1. Realizar la división por 16
     1. $58 / 16 = 3  \rightarrow 58 - (16 * 3) = 58 - 48 = 10$
     2. $3 / 16 = 0 \rightarrow 3 - (16 * 0) = 3 - 0 = 3$
  2. Se Toman los digitos de abajo hacia arriba, y se ordenan de izquierda a derecha, cambiando los mayores a 9 por sus respectivas letras
     1. $3$ $10$ $\rightarrow 3\text{A}$

- [X] a) 3A
- [ ] b) B7
- [ ] c) 3B
- [ ] d) 4A
- [ ] e) 15


<br><br>

#### Considere el siguiente valor Binario representado en complemento a uno, en un registro de memoria de 8 bits y encuentre su correspondiente valor decimal (4.5)

    1011 0011


#### Solución

Nos damos cuenta que nos dicen complemento a uno, y que el bit más significativo esta representado por **1**, con esto podemos concluir que el numero a representar si es negativo, luego, sebemos invertir los digitos para tener el mismo numero, en representación positiva.

1. Invirtiendo:
   1. $1011 0011 \rightarrow 01001100$
   2. $64 + 8 + 4$
   3. $76$
2. Al tener el bit mas significativo en 1:
   1. $- 76$

- [ ] a) 98
- [ ] b) 179
- [ ] c) 76
- [ ] d) la alternativa correcta no se encuentra listada
- [X] e) -76

<br><br>

#### Cual es la equivalencia Hexadecimal del siguiente valor Binario (4.5)

    111010

#### Solución 1:
  1. Tomar grupos de 4 bits, desde derecha a izquierda:
     1. Grupos: $11$ y $1010$
  2. Luego, convertir esos grupos a su valor decimal:
     1. $11 \rightarrow 2 + 1 = 3$
     2. $1010 \rightarrow 8 + 2 = 10$
  3. Como Hexadecimal representa digitos de 0-9 y letras de A-F, transormamos el 10 a su letra correspondiente, quedando:
     - $1010 \rightarrow 8 + 2 = 10 \rightarrow \text{A}$
  4. Finalmente, juntamos: 
     - $3\text{A}$ 

#### Solución 2:

  1. Tranformar el valor binario a decimal:
     1. $111010 \rightarrow 32 + 16 + 8 + 2 = 58$
  2. Realizar la división por 16
     1. $58 / 16 = 3  \rightarrow 58 - (16 * 3) = 58 - 48 = 10$
     2. $3 / 16 = 0 \rightarrow 3 - (16 * 0) = 3 - 0 = 3$
  2. Se Toman los digitos de abajo hacia arriba, y se ordenan de izquierda a derecha, cambiando los mayores a 9 por sus respectivas letras
     1. $3$ $10$ $\rightarrow 3\text{A}$

- [ ] a) 240
- [ ] b) F1
- [ ] c) D1
- [X] d) 3A
- [ ] e) A0


<br><br>

#### Demuestre y obtenga el resultado binario, de la siguiente operación (4.5)

    111101 / 11

#### Solución:

&nbsp;1 1 1 1 0 1 / 11 = 10100
-1 1
0 0 1
0 0 1 1
&nbsp; &nbsp; - 1 1
&nbsp; &nbsp; &nbsp; 0 0 0
&nbsp; &nbsp; &nbsp; 0 0 0 1