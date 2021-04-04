# Python

Web: https://www.python.org/

## Comentarios
```python
# Esto es un comentario

'''
Comentario de varias
líneas
o
Doc String con triple comillas simple
'''

"""
Comentario de varias
líneas
o
Doc String con triple comillas
"""
```

## Variables

```python
nombre = 'Pedro'
edad = 27;

print('Hola',nombre)
print('Tu edad es', edad)

type(nombre)
```

## Tipos de datos

str
int
float
bool (True / False)

## Operadores

### Asignación
=
+=
-=
*=
/=
//=
%=
**=

### Aritméticos
Suma +
Resta -
Multiplicación *
División /
División Entera //
Módulo %
Potencia **



## IF

```python
if x < 0:
    x = 0
    print('Negativo cambiado a cero')
```


## IF-ELSE
```python
if x < 0:
    x = 0
    print('Negativo cambiado a cero')
else:
    print('Positivo o cero')
```

## ELIF
```python
if x < 0:
    x = 0
    print('Negativo cambiado a cero')
elif x == 0:
    print('Cero')
elif x == 1:
    print('Uno')
else:
    print('Mayor')
```

## WHILE
```python
a, b  = 0, 1

while a < 10:
    print(a)
    a, b = b, a+b
```

## FOR
```python
lista = ['elemento1', 'elemento2', 'elemento3']

for elemento in lista:
    print('Item:', elemento)
```

break
no se puede usar el else

## Funciones
```python
def miFuncion():
    print
```
