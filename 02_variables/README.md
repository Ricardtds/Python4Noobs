# Variáveis
Variáveis são containers para guardar valores de dados

## Criando variáveis
O python não possui forte tipagem para declarar um variável. A variáve é criada no momento que você atribui um valor a ela.

```
x  = 5
y = "John"
print(x)
print(y)
```

## Casting
Se você deejar específicar o tipo da variável
```
x = str(3) # x será '3'
y = int(3) # y será 3
z = float(3) # z será 3.0
```

## Get the Type
A função type() retorna o tipo da variáve
```
x = 5
y = "John"
print(type(x))
print(type(y)) 
```

## Single or Double Quotes?
As strings podem ser declaradas usando ' ou ".
```
x = "Ricardo"
# é o mesmo que
x = 'Ricardo'
```

## Case-Sensitive
As variáveis são sensíveis a letras maiúsculas e minúsculas
```
a = 4
A = "Pedro"
# A e a representam duas variáveis diferentes.
```

# Nomes de variáveis
As regras para os nomes de variáveis são:
+ A variável deve começar com uma letra ou com o _
+ A variável não pode começar com um número
+ A variável só pode conter alfanumérico e _ (A-z, 0-9 e _)
+ Os nomes de variável são case-sensitive
+ A variável não pode ser um nome reservado

Exemplos válidos:
```
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```

## Multi Words Variable Names
Camel case:
```
myVariableName = "John" 
```
Pascal Case:
```
MyVariableName = "John" 
```
Snake Case:
```
my_variable_name = "John" 
```

# Assign Multiple Values

## Many Values to Multiple Variables
Python permite que você dê valores a várias variáveis usando uma única linha.
```
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```

## One Value to Multiple Variabels
Python permite que você dê o mesmo valor a várias variáveis usando uma única linha.
```
x = y = z = "Orange"
print(x)
print(y)
print(z)
```
## Unpack a Collection
Se você tiver uma coleção de valores em uma lista, tupla etc. Você pode desempacotar.

```
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
```

# Output Variables
O print é uma função muito usada para imprimir valores.
```
x = "Python is awesome"
print(x)
```
Você pode imprimir vária variávei separadas por vírgulas.
```
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
```
Para números o operador + trabalha como um operador matemático
```
x = 5
y = 10
print(x + y)
```

# Global Variable
As variávei criadas fora de uma função (como abaixo) são conhecidas como variáveis globais. Elas podem ser usadas em qualquer parte do código.

```
x = "awesome"

def myfunc():
  print("Python is " + x)

myfunc() 
```

Uma variável criada dentro de uma função é uma variável local e só pode ser utilizada dentro da função.
```
x = "awesome"

def myfunc():
  x = "fantastic"
  print("Python is " + x)

myfunc()

print("Python is " + x) 
```

Para fazer com que não seja criado uma nova variável dentro da função e sim seja utilizada a de fora usamos o termo global.

```
x = "awesome"

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x) 
```