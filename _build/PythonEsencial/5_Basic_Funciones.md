---
redirect_from:
  - "/pythonesencial/5-basic-funciones"
interact_link: content/PythonEsencial/5_Basic_Funciones.ipynb
kernel_name: python3
has_widgets: false
title: 'Basic Funciones'
prev_page:
  url: /PythonEsencial/4_Basic_EstructurasdeControl
  title: 'Basic Estructurasdecontrol'
next_page:
  url: /PythonEsencial/1_Basic_Aritmética
  title: 'Basic Aritmética'
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

**funciones**
- - -



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
def f(x):
    print ("El argumento x =",x)
    return 2*x

```
</div>

</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
f(3)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
El argumento x = 3
```
</div>
</div>
<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
6
```


</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
f(3.5)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
El argumento x = 3.5
```
</div>
</div>
<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
7.0
```


</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
f("hola")

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
El argumento x = hola
```
</div>
</div>
<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
'holahola'
```


</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
def f(x):
    print ("El argumento x =",x)
    return x*x

```
</div>

</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
f(2.5)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
El argumento x = 2.5
```
</div>
</div>
<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
6.25
```


</div>
</div>
</div>



** Funciones de varios argumentos **



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
def f(x,y):
    return 2*x, 3*y

```
</div>

</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
f(3,5)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
(6, 15)
```


</div>
</div>
</div>



**Funciones con documentación**



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
def cuad(x):
    """
    Función que evalúa el cuadrado de un número.
    Funciona siempre y cuando el tipo de variable x permita multiplicarlo por si mismo.
    """
    return x*x

```
</div>

</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
cuad(2)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
4
```


</div>
</div>
</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
cuad?

```
</div>

</div>



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
cuad(1+1J)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">


{:.output_data_text}
```
2j
```


</div>
</div>
</div>



** Ejercicio.** Escribe una función que calcule el volumen de una esfera 
al dar como argumento el radio.



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
def V(r):
    π = 3.14159265
    return 4/3*π*r*r*r

```
</div>

</div>

