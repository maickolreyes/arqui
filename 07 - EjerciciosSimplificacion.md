# Ejercicios

### Simplifique usando Morgan y Karnaugh
1. $\overline{(AC + \overline{B}D)(B + \overline{CD})}$

R: 
   - Ecuacion simplificada deMorgan: $\bar{A}B + \bar{A}\bar{D} + B\bar{C} + \bar{C}\bar{D} + \bar{B}CD$
   - Simplficacion despues de Karnaugh: $\bar{A}C + B\bar{C} + \bar{C}\bar{D} + \bar{B}CD$

<br>

2. $\overline{\bar{A}(C + D) + \bar{B}(A + D) + \bar{A} \bar{B} \bar{C}}$

R: 
   - Ecuacion simplificada deMorgan: $AB + AB + ABC + AB\bar{C}\bar{D} + B\bar{C}\bar{D} + \bar{A}B\bar{C}\bar{D}$
   - Simplficacion despues de Karnaugh: $AB + B\bar{C}\bar{D}$
<br>

3. $\overline{(A + B)} * \overline{(A + BC)} * [A + (AC + B)]$

R: 
   - Ecuacion simplificada deMorgan: $0$
   - Simplficacion despues de Karnaugh:$0$ 

<br>

### Simplifique usando Boole y Morgan
1. $\overline{\overline{(AB + BC)} + (AC + \overline{B})}$

R:
   - Ecuacion simplificada: $AB\bar{C} + \bar{A}BC$

<br> 

2. $\overline{\bar{A}(C + D) + \bar{B}(A + D) + \bar{A} \bar{B} \bar{C}}$

R:
   - Ecuacion simplificada: $AB + B\bar{C}\bar{D}$

<br>

3. $(B + BA + BCA) * \overline{(\bar{B} + \bar{A})} * (CB + \bar{C}A + \bar{C})$

R:
   - Ecuacion simplificada: $AB$

<br>

### Simplifique dado una tabla de verdad
1. 

| A | B | C | S |
|---|---|---|---|
| 0 | 0 | 0 | 1 |
| 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |
| 1 | 1 | 1 | 1 |

R:
   - Ecuacion simplificada: $\bar{A} + BC$