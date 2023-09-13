# Strings
Strins em python são cercadas por ' ou ".

'hello" é o mesmo que "hello"

## Assign String to a Variable

```
a = "Hello"
print(a)
```

## Multiline Strings
Você pode atribuir uma string de várias linhas em uma variável usando três "

```
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a) 
```
ou usando três '
```
a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a) 
```

## Strings are Arrays
Python não possui o tipo de dado character, um único caractere é simplesmente uma string de tamanho 1.
Podemos aessar o elemento usando o [index].

```
a = "Hello, World!"
print(a[1]) # imprime e
```

## Looping Through a String
Como Strings são arrays, podemos:

```
for x in "banana":
  print(x)
```

## String Length
Para obter o tamanho da string utilizamos a função len()

```
a = "Hello, World!"
print(len(a))
```

## Check String
Para verificar se certa frase ou letra está presente na string podemos usar a palavra-chave _in_

```
txt = "The best things in life are free!"
print("free" in txt) # True
```

# Slicing Strings
Podemos retornar uma faixa de caracteres usando a sintaxe slice

```
b = "Hello, World!"
print(b[2:5]) # a posição 5 não é inclusa
```

## Slice From the Start
```
b = "Hello, World!"
print(b[:5])
```

## Slice To the End
```
b = "Hello, World!"
print(b[2:])
```

## Negative Indexing
Use índices negativos para iniciar a fatia do final da string:

```
b = "Hello, World!"
print(b[-5:-2])
```