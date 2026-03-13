### Operadores

Em Python, os operadores são símbolos especiais usados para realizar operações com variáveis e valores. Eles formam a base das expressões que compõem a lógica dos programas e estão divididos em diferentes categorias, entre as quais destacamos: aritméticos, relacionais, lógicos e de atribuição.

Os operadores aritméticos são utilizados para realizar cálculos matemáticos. Com eles, podemos somar (+), subtrair (-), multiplicar (*), dividir (/), calcular o resto da divisão (%), a divisão inteira (//) e potências (**).

Já os operadores relacionais comparam valores e retornam um resultado booleano (True ou False). São eles: igual (==), diferente (!=), maior que (>), menor que (<), maior ou igual (>=) e menor ou igual (<=). São fundamentais para expressar condições em programas.

Os operadores lógicos permitem combinar ou inverter expressões booleanas. Usamos and (e lógico), or (ou lógico) e not (negação) para construir condições compostas, essenciais em estruturas como if.

Por fim, os operadores de atribuição são usados para atribuir valores a variáveis. Além do = simples, há formas abreviadas que combinam atribuição com operações, como +=, -=, *=, entre outros, que facilitam a atualização de valores.

Compreender e dominar esses operadores é essencial para escrever expressões corretas, tomar decisões e controlar o fluxo de execução nos programas em Python.

### Operadores aritméticos

Em Python, os operadores aritméticos servem para realizar cálculos com números. Por exemplo, se quisermos somar dois valores, basta usar o símbolo +. Da mesma forma, usamos - para subtração, * para multiplicação e / para divisão. Veja este exemplo simples:

Note que, no caso da divisão com /, o resultado será sempre um número do tipo float, mesmo que a divisão seja exata.

```python
a = 10
b = 3

soma = a + b       # 13
subtracao = a - b  # 7
multiplicacao = a * b  # 30
divisao = a / b    # 3.333...
```

Se você quiser obter apenas o quociente inteiro da divisão, ou seja, sem a parte decimal, pode usar o operador //. Esse operador é útil quando queremos saber quantas vezes um número "cabe" dentro de outro, como em divisões inteiras. Por exemplo:

```python 
divisao_inteira = a // b  # 3
```

Outro operador importante é o módulo, representado por %, que retorna o resto da divisão. Ele é muito utilizado, por exemplo, para verificar se um número é par ou ímpar:
```python 
resto = a % b  # 1
eh_par = a % 2 == 0  # True, porque 10 é par
```

Por fim, temos o operador de exponenciação, **, que eleva um número a uma determinada potência. Se quisermos calcular 2 elevado a 3, por exemplo, fazemos:

```python 
potencia = 2 ** 3  # 8
```

Em Python (assim como em matemática), a ordem de precedência dos operadores aritméticos é a seguinte:

1. Parênteses ()
2. Exponenciação **
3. Multiplicação *, Divisão /, Divisão inteira //, Módulo % (da esquerda para a direita)
4. Adição + e Subtração - (também da esquerda para a direita) 

Vamos ver isso em prática com alguns exemplos comentados:
Expressão simples

:::info

```
resultado = 2 + 3 * 4
print(resultado)  # Resultado: 14
```
:::tip
Aqui, a multiplicação acontece antes da soma. 
Primeiro é feito 3 * 4 = 12, depois 2 + 12 = 14.
::: 

Alterando a precedência com parênteses
```
resultado = (2 + 3) * 4
print(resultado)  # Resultado: 20
```
:::tip
Com parênteses, o Python soma primeiro 2 + 3 = 5, e só depois multiplica por 4.
::: 

Incluindo módulo e exponenciação
```
resultado = (2 + 3) ** 2 % 4
print(resultado)  # Resultado: 1
``` 

Aqui temos:
```
2 + 3 = 5
5 ** 2 = 25
25 % 4 = 1
```

Expressões mais encadeadas
```
a = 10
b = 3
c = 2
​resultado = a * b - a // c + a % b
print(resultado)  # Resultado: 30 - 5 + 1 = 26
```
A ordem é:
```
a * b = 10 * 3 = 30
a // c = 10 // 2 = 5
a % b = 10 % 3 = 1
```
resultado = 30 - 5 + 1 = 26

:::
