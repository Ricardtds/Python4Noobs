# Operators
Py thon divides os operadores nos seguintes grupos:

+ Operadores aritméticos
+ Operadores de atribuição
+ Operadores de comparação
+ Operadores lógicos
+ Operadores de identidade
+ Operadores de associação
+ Operadores bit a bit

## Operadores aritméticos
Operadores aritméticos são usados com valores numéricos para realizar operações matemáticas comuns
| Operator | Name | Example |
| - | - | - |
| + | Addition | x + y 	|
| - | Subtraction | x - y |	
| * | Multiplication | x * y |	
| / | Division | x / y |
| % | Modulus | x % y |
| ** | Exponentiation |	x ** y| 	
| // | Floor division | x // y|

## Operadores de atribuição
Operadores de atribuição são usados para atribuir valores a variáveis
| Operator | Example |   Same As |
| - | - | - |
| = 	| x = 5 	|   x = 5 	|
| += 	| x += 3 	|   x = x + 3 	|
| -= 	| x -= 3 	|   x = x - 3 	|
| *= 	| x *= 3 	|   x = x * 3 	|
| /= 	| x /= 3 	|   x = x / 3 	|
| %= 	| x %= 3 	|   x = x % 3 	|
| //= 	| x //= 3 	|   x = x // 3 	|
| **= 	| x **= 3 	|   x = x ** 3 	|
| &= 	| x &= 3 	|   x = x & 3 	|
| \|= 	| x \|= 3 	|   x = x \| 3 	|
| ^= 	| x ^= 3 	|   x = x ^ 3 	|
| >>= 	| x >>= 3 	|   x = x >> 3 	|
| <<= 	| x <<= 3 	|   x = x << 3  |

## Operadores de comparação
Operadores de comparação são usados para comparar dois valores
| Operator | Name | Example |
| - | - | - |
| == |	Equal | x == y 	
| != |	Not equal | x != y 	
| > |	Greater than | x > y 	
| < |	Less than | x < y 	
| >= |	Greater than or equal to | x >= y 	
| <= |	Less than or equal to | x <= y

## Operadores lógicos
Operadores lógicos são usados para combinar instruções condicionais
| Operator |	Description	| Example |
| - | - | - |
| and | Returns True if both statements are true | x < 5 and  x < 10 	
| or |	Returns True if one of the statements is true | x < 5 or x < 4 	
| not |	Reverse the result, returns False if the result is true | not(x < 5 and x < 10)

## Operadores de identidade
Os operadores de identidade são usados para comparar os objetos, não se forem iguais, mas se forem realmente o mesmo objeto, com a mesma localização de memória
| Operator | Description | Example |
| - | - | - |
| is | 	Returns True if both variables are the same object |	x is y 	
| is not | Returns True if both variables are not the same object |	x is not y

## Operadores de associação
Operadores de associação são usados para testar se uma sequência é apresentada em um objeto
| Operator |	Description |	Example |
| - | - | - |
| in | 	Returns True if a sequence with the specified value is present in the object |	x in y 	
| not in |	Returns True if a sequence with the specified value is not present in the object | x not in y

## Operadores bit a bit
Operadores bit a bit são usados para comparar números (binários)

| Operator | Name | Description | Example
| - | - | - | - |
| & | AND |	Sets each bit to 1 if both bits are 1 |x & y 	
| \| | OR |	Sets each bit to 1 if one of two bits is 1 | x \| y 	
| ^ |	XOR |	Sets each bit to 1 if only one of two bits is 1 |	x ^ y 	
| ~ |	NOT |	Inverts all the bits |	~x 	
| << |	Zero fill left shift |	Shift left by pushing zeros in from the right and let the leftmost bits fall off |	x << 2 	
| >> |	Signed right shift |	Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off |	x >> 2

## Operator Precedence
A precedência do operador descreve a ordem em que as operações são executadas.

A ordem de precedência está descrita na tabela abaixo, começando com a precedência mais alta no topo:

| Operator |	Description |
| - | - |
| () |	Parentheses 	
| ** |	Exponentiation 	
| +x  -x  ~x |	Unary plus, unary minus, and bitwise NOT 	
| *  /  //  % |	Multiplication, division, floor division, and modulus 	
| +  - |	Addition and subtraction 	
| <<  >> |	Bitwise left and right shifts 	
| & |	Bitwise AND 	
| ^  |	Bitwise XOR 	
| | |	Bitwise OR 	
| ==  !=  >  >=  <  <=  is  is not  in  not in  |	Comparisons, identity, and membership operators 	
| not |	Logical NOT 	
| and |	AND 	
| or |	OR