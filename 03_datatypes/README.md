# Python Data Types

## Built-in Data Types
O python tem os seguintes tipos de dados por padrão.

| Categories | Types |
| - | - |
| Text Type | str |
| Numeric Types | int, float, complex |
| Sequence Types | list, tuple, range |
| Mapping Type | dict |
| Set Types | set, frozenset |
| Boolean Type | bool |
| Binary Types | bytes, bytearray, memoryview |
| None Type | NoneType |

## Getting the Data Type
Você pode obter o tipo de dado de qualquer objeto utilizando a função type()
```
x = 5
print(type(x))
```

## Setting the Data Type
| Example | Data Type |
| - | - |
| x = "Hello World" | str |
| x = 20 | int |
| x = 20.5 | float |
| x = 1j | complex |
| x = ["apple", "banana", "cherry"] | list |
| x = ("apple", "banana", "cherry") | tuple |
| x = range(6) | range |
| x = {"name" : "John", "age" : 36} | dict |
| x = {"apple", "banana", "cherry"} | set |
| x = frozenset({"apple", "banana", "cherry"}) | frozenset |
| x = True | bool |
| x = b"Hello" | bytes |
| x = bytearray(5) | bytearray |
| x = memoryview(bytes(5)) | memoryview |
| x = None | NoneType |


## Setting the Specific Data Type
| Example | Data Type |
| -  | - |
|x = str("Hello World") |	str 	|
|x = int(20) |	int 	|
|x = float(20.5) |	float 	|
|x = complex(1j) |	complex 	|
|x = list(("apple", "banana", "cherry")) |	list 	|
|x = tuple(("apple", "banana", "cherry")) |	tuple 	|
|x = range(6) |	range 	|
|x = dict(name="John", age=36) |	dict 	|
|x = set(("apple", "banana", "cherry")) |	set 	|
|x = frozenset(("apple", "banana", "cherry")) |	frozenset 	|
|x = bool(5) |	bool 	|
|x = bytes(5) |	bytes 	|
|x = bytearray(5) |	bytearray 	|
|x = memoryview(bytes(5)) |	memoryview |

# Numbers 
Existem tres tipos numéricos em python:
+ int | são números inteiros sem decimais
+ float | são números flutuantes com decimais
+ complex | são números que contem a parte imaginária

```
x = 1    # int
y = 2.8  # float
z = 1j   # complex
```

## Type conversion
```
.
.
.
#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)
.
.
.
```
[Type Conversion example code](/03_datatypes/typeconversion.py)

> Nota: Você não pode converter números complexos em outro tipo de número.

## Random Number
O python possui um módulo chamado random que pode ser utilizado para gerar números aleatórios.

```
"""
O código importa o módulo random
Utiliza a função randrange(x,y) do módulo gerando números aleatórios de x a y
"""
import random

print(random.randrange(1, 10))
```

# Casting

## Specify a Variable Type

Pode haver momentos em que você queira especificar um tipo para uma variável. Isso pode ser feito com fundição. Python é uma linguagem orientada a objetos e, como tal, usa classes para definir tipos de dados, incluindo seus tipos primitivos.

A conversão em python é, portanto, feita usando funções construtoras:

+ int() - constrói um número inteiro a partir de um literal inteiro, um literal flutuante (removendo todos os decimais) ou um literal de string (desde que a string represente um número inteiro)

+ float() - constrói um número float a partir de um literal inteiro, um literal float ou um literal de string (desde que a string represente um float ou um inteiro)

+ str() - constrói uma string a partir de uma ampla variedade de tipos de dados, incluindo strings, literais inteiros e literais flutuantes

Example:

| Integers | Floats | Strings |
| - | - | - |
| x = int(1)   # x will be 1 |  x = float(1) # x will be 1.0 | x = str("s1") # x will be 's1'
| y = int(2.8) # y will be 2 | y = float(2.8)   # y will be 2.8 | y = str(2)    # y will be '2'
| z = int("3") # z will be 3 | z = float("3")   # z will be 3.0 | z = str(3.0)  # z will be '3.0'
 | | w = float("4.2") # w will be 4.2