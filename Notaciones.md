# Notaciones Posicionales

## **Binario** 

---------------------------
- Nos indican posición de datos y se leen en potencias de 2 según el orden que poseen:

    |$2^{7}$|$2^{6}$|$2^{5}$|$2^{4}$|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
    |-------|-------|-------|-------|-------|-------|-------|-------|
    |  128  |   64  |   32  |   16  |   8   |   4   |   2   |   1   |

    **Convertir:** Binario -> Decimal

    00101101

    |$2^{7}$|$2^{6}$|$2^{5}$|$2^{4}$|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
    |-------|-------|-------|-------|-------|-------|-------|-------|
    |   0   |   0   |   1   |   0   |   1   |   1   |   0   |   1   |
    |  128  |  64   |   32  |   16  |   8   |   4   |   2   |   1   |

* 00101101 -> $0*2^{7} + 0*2^{6} + 1*2^{5} + 0*2^{4} + 1*2^{3} + 1*2^{2} + 0*2^{1} + 1*2^{0}$
* 00101101 -> $0*128 + 0*64 + 1*32 + 0*16 + 1*8 + 1*4 + 0*2 + 1*1$
* 00101101 -> $32 + 8 + 4 + 1$
* 00101101 -> $45$

    **Convertir:** Decimal -> Binario

    234

    - Descomposición en potencias de 2 hasta llegar a 0: 
      - $234 - 128 = 106$
      - $106 - 64 = 42$
      - $42 - 32 = 10$
      - $10 - 8 = 2$
      - $2 - 2 = 0$  
  
    - Identificando los valores:
      - 128 / 64 / 32 / 8 / 2

    - Se ubican esos valores en la **posicion** o **potencia** correspondiente:
      - $2^7$ / $2^6$ / $2^5$ / $2^3$ / $2^1$

    - Esas posicion se **activan** o **cambian su estado** correspondiente:
    
        |$2^{7}$|$2^{6}$|$2^{5}$|$2^{4}$|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
        |-------|-------|-------|-------|-------|-------|-------|-------|
        |   0   |   0   |   0   |   0   |   0   |   0   |   0   |   0   |

  - El binario anterior pasaria a ser:
   
    |$2^{7}$|$2^{6}$|$2^{5}$|$2^{4}$|$2^{3}$|$2^{2}$|$2^{1}$|$2^{0}$|
    |-------|-------|-------|-------|-------|-------|-------|-------|
    |   1   |   1   |   1   |   0   |   1   |   0   |   1   |   0   |
  
  - Dando como resultado:
    - 234 -> 11101010

## **Octal**

-----------------------

- Nos indican posicionamiento con numeraciones del 0 - 7. Y la diferencia con la notacion binaria es la representacion en potencias de 8:

    |$8^{7}$|$8^{6}$|$8^{5}$|$8^{4}$|$8^{3}$|$8^{2}$|$8^{1}$|$8^{0}$|
    |-------|-------|-------|-------|-------|-------|-------|-------|
    |2097152| 262144| 32768 |  4096 |  512  |  64   |   8   |   1   |


    **Convertir:** Octal -> Decimal

    $623_{(8)}$

    - Se realizan pasos similares al binario, es decir, dígito por la potencia de 8 correspondiente a la ubicacion del dígito:

      - $623_{(8)}$ -> $6 * 8^2$ + $2*8^1$ + $3*8^0$
      - $623_{(8)}$ -> $6 * 64$ + $2*8$ + $3*1$
      - $623_{(8)}$ -> $384$ + $16$ + $3$
      - $623_{(8)}$ -> $403$  
   
    **Convertir:** Decimal -> Octal

    $95$
    - Realizar un ciclo repetitivo de divisiones hasta llegar a 0 **(División entera, NO decimales)**
      - $95$ -> $95/8 = 11$ Sobran $95-(8*11) = 7$
    - Se sigue trabajando con el resultado de la división por 8 y al finalizar la operación se toman todos los restos de las divisiones y se agrupan desde el último al primero de izquierda a derecha
      - $95$ -> $11/8 = 1$ Sobran $11 - (8*1) = 3$
      - $95$ -> $1/8 = 0$ Sobran $ 1 - (8*0) = 1$
    - Tomando el resto de la divisiones el numero quedaría como:
      - $95$ -> $137_{(8)}$


## Hexadecimal
-------

