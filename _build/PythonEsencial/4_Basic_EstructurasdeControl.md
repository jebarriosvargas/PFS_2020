---
redirect_from:
  - "/pythonesencial/4-basic-estructurasdecontrol"
interact_link: content/PythonEsencial/4_Basic_EstructurasdeControl.ipynb
kernel_name: python3
has_widgets: false
title: 'Basic Estructurasdecontrol'
prev_page:
  url: /intro
  title: 'Intro'
next_page:
  url: /PythonEsencial/5_Basic_Funciones
  title: 'Basic Funciones'
comment: "***PROGRAMMATICALLY GENERATED, DO NOT EDIT. SEE ORIGINAL FILES IN /content***"
---
<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
from IPython.core.display import display, HTML
display(HTML("<style>.container { width:95% !important; }</style>"))

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">

<div markdown="0" class="output output_html">
<style>.container { width:95% !important; }</style>
</div>

</div>
</div>
</div>



- - - 
# Contenido
**if** (*si...*)

**for** (*en cada ...*)

**while** (*mientras...*)
- - -



## if (condición)



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
a=10
if(a>10):
    print("El valor es mayor a 10.")
else :
    print("El valor de a es menor o igual a 10.")

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
El valor es mayor a 10.
```
</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
x = False
y = True

if x and y:
    print('Tanto x como y son True')
else:
    print('x es False o y es False o tanto x y y son False')
print ()
if x or y:
    print('x es True o y es True o tanto x y y son True')
else:
    print('Tanto x como y son False')

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
x es False o y es False o tanto x y y son False

x es True o y es True o tanto x y y son True
```
</div>
</div>
</div>



**Ejercicio** Escribir utilizando `if` el valor absoluto de una variable a.



--- 



## for (iteración sobre listas)



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
colores = ["Red", "Blue", "Green", "Black"]

```
</div>

</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
for c in colores:
    print (c)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
Red
Blue
Green
Black
```
</div>
</div>
</div>



**función** `range( )`



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
range(4)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
range(0, 4)
```


</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
for a in range(4):
    print (a)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
0
1
2
3
```
</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
for a in range(2,7):
    print(a)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
2
3
4
5
6
```
</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
for a in range(2,19,5):
    print(a)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
2
7
12
17
```
</div>
</div>
</div>



**Escritura en formato latex** `$   $`

$\int e^{x^2} dx$



**Ejercicio.** Encuentre los primeros 3 números de Fibonacci.

$f_0=0,\quad f_1=1,\quad f_n = f_{n-1}+f_{n-2}$



**Ejercicio.** Encuentre los primeros 100 números de Fibonacci.

$f_0=0,\quad f_1=1,\quad f_n = f_{n-1}+f_{n-2}$



---



## while (ciclo hasta que se cumple una condición)



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
i = 0
while i<10:
    i += 1
    print (i)

```
</div>

</div>



**¡CUIDADO!**



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
i = 0
while i<10:
    i +=1
    print (i)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
1
2
3
4
5
6
7
8
9
10
```
</div>
</div>
</div>



**Ejercicio.** Encuentre los números de Fibonacci menores que 100.

$f_0=0,\quad f_1=1,\quad f_n = f_{n-1}+f_{n-2}$



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
fnm2 = 0
fnm1 = 1
while ((fnm1 + fnm2)<100):
    fn   = fnm1 + fnm2
    fnm2 = fnm1
    fnm1 = fn
    print (fn)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
1
2
3
5
8
13
21
34
55
89
```
</div>
</div>
</div>



**Ejercicio.** Implementa el método babilónico para calcular la raíz cuadrada 
de un número dado $y$ Este método consiste en la iteración $x_{n+1}=\frac{1}{2}\big[x_n + y/x_n \big]$. ¿Qué tan rápido converge?

