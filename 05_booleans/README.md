# Booleans

Booleans representam um dos dois valores: True ou Falso.

## Boolean Values
Na programação você precisa frequentemente saber se uma expressão é verdadeira ou falsa.

```
a = 200
b = 33

if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a") 
```

## Evaluate Values and Variables
A função bool() permite avaliar qualquer valor e retorne True ou False.

```
x = "Hello"
y = 15

print(bool(x))
print(bool(y))
```

## Most Values are True
Quase qualquer valor é avaliado como True se tiver algum tipo de conteúdo.

+ Qualquer string é True, exceto strings vazias.
+ Qualquer número é True, exceto o 0.
+ Qaulquer lista, tuple, set e dicionário são True, exceto os vazios.