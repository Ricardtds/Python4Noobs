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

# Modify Strings

## Upper Case
O método upper() retorna a string em caixa alta:
```
a = "Hello, World!"
print(a.upper()) # HELLO, WORLD!
```

## Lower Case
O método lower() retorna a string em caixa baixa:
```
a = "Hello, World!"
print(a.lower()) # hello, world!
```

## Remove Whitespace
Espaços em brancos são espaçoes antes/ou depois do texto atual, é muito comum você querer remover este espaço.

O método strip() removes qualquer espaço em branco do ínicio ou do final.
```
a = " Hello, World! "
print(a.strip()) # returns "Hello, World!" 
```

## Replace string
O método replace() troca uma string com outra string.
```
a = "Hello, World!"
print(a.replace("H", "J"))
```

## Split String
O método split() retorna uma lista onde o texto entre o separador específicado se torna uma lista de itens.
```
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!'] 
```

## String Concatenation
Para concatecar our combinar duas strings você pode usar o operador +

```
a = "Hello"
b = "World"
c = a + b
print(c) # HelloWorld
```

## String Format
Nós não podemos combinar strings com números no método de cima. Mas nós podemos ombinar strings  e números usando o método format()

O método format() pega os argumentos passados, formata-os e os coloca na string onde estão os espaços reservados {}

```
quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price)) # I want 3 pieces of item 567 for 49.95 dollars.
```

Você pode usar números de índice {0} para garantir que os argumentos sejam colocados nos espaços reservados corretos

```
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price)) # I want to pay 49.95 dollars for 3 pieces of item 567.
```

## Escape Character
Para inserir caracteres "ilegais" em uma string, use um caractere de escape.
```

```

## Escape Characters
| Code | Result |
| - | - |
| \\' | 	Single Quote 	|
| \\\ | 	Backslash 	|
| \n | 	New Line 	|
| \r | 	Carriage Return 	|
| \t | 	Tab 	|
| \b | 	Backspace 	|
| \f | 	Form Feed 	|
| \ooo | 	Octal value 	|
| \xhh | 	Hex value |

## String Methods
Todos os métodos retornam novos valores. Eles não alteram a string original.
| Method | Description |
| - | - |
| capitalize() |	Converte o primeiro caractere para maiúsculo |
| casefold() |	Converte string em minúsculas |
| center() |	Retorna uma string centralizada |
| count() |	Retorna o número de vezes que um valor especificado ocorre em uma string |
| encode() |	Retorna uma versão codificada da string |
| endswith() |	Retorna verdadeiro se a string terminar com o valor especificado |
| expandtabs() |	Define o tamanho da tabulação da string |
| find() |	Pesquisa a string por um valor especificado e retorna a posição onde ele foi encontrado |
| index() |	Pesquisa a string por um valor especificado e retorna a posição onde ele foi encontrado |
| format() |	Formata valores especificados em uma string |
| format_map() |	Formata valores especificados em uma string |
| isalnum() |	Retorna True se todos os caracteres da string forem alfanuméricos |
| isalpha() |	Retorna True se todos os caracteres da string estiverem no alfabeto |
| isascii() |	Retorna True se todos os caracteres da string forem caracteres ASCII |
| isdecimal() |	Retorna True se todos os caracteres da string forem decimais |
| isdigit() |	Retorna True se todos os caracteres da string forem dígitos |
| isidentifier() |	Retorna True se a string for um identificador |
| islower() |	Retorna True se todos os caracteres da string estiverem em minúsculas |
| isnumeric() |	Retorna True se todos os caracteres da string forem numéricos |
| isprintable() |	Retorna True se todos os caracteres da string puderem ser impressos |
| isspace() |	Retorna True se todos os caracteres da string forem espaços em branco |
| istitle() | Retorna True se a string segue as regras de um título |
| isupper() |	Retorna True se todos os caracteres da string estiverem maiúsculos |
| join() |	Une os elementos de um iterável ao final da string |
| ljust() |	Retorna uma versão justificada à esquerda da string |
| lower() |	Converte uma string em minúsculas |
| lstrip() |	Retorna uma versão cortada à esquerda da string |
| maketrans() |	Retorna uma tabela de tradução para ser usada nas traduções |
| partition() |	Retorna uma tupla onde a string é dividida em três partes |
| replace() |	Retorna uma string onde um valor especificado é substituído por um valor especificado |
| rfind() |	Pesquisa a string por um valor especificado e retorna a última posição de onde foi encontrado |
| rindex() |	Pesquisa a string por um valor especificado e retorna a última posição de onde foi encontrado |
| rjust() |	Retorna uma versão justificada à direita da string |
| rpartition() |	Retorna uma tupla onde a string é dividida em três partes |
| rsplit() |	Divide a string no separador especificado e retorna uma lista |
| rstrip() |	Retorna uma versão aparada à direita da string |
| split() |	Divide a string no separador especificado e retorna uma lista |
| splitlines() |	Divide a string nas quebras de linha e retorna uma lista |
| startswith() |	Retorna verdadeiro se a string começar com o valor especificado |
| strip() |	Retorna uma versão aparada da string |
| swapcase() |	Troca de maiúsculas, minúsculas tornam-se maiúsculas e vice-versa |
| title() |	Converte o primeiro caractere de cada palavra para maiúscula |
| translate() |	Retorna uma string traduzida |
| upper() |	Converte uma string em maiúscula |
| zfill() |	Preenche a string com um número especificado de valores 0 no início |