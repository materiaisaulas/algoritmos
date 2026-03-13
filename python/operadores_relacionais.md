### Operadores Relacionais

:::info
Os **operadores relacionais** são utilizados para **comparar dois valores**.  
Eles retornam sempre um resultado lógico:

- `True` (verdadeiro)
- `False` (falso)
:::

Esses operadores são fundamentais em **estruturas condicionais**, como `if`, e em **laços de repetição**, como `while`.

### Tabela de operadores relacionais

| Operador | Significado | Exemplo | Resultado |
|----------|-------------|--------|-----------|
| `==` | Igual a | `5 == 5` | `True` |
| `!=` | Diferente de | `3 != 4` | `True` |
| `>` | Maior que | `7 > 2` | `True` |
| `<` | Menor que | `2 < 1` | `False` |
| `>=` | Maior ou igual a | `10 >= 10` | `True` |
| `<=` | Menor ou igual a | `8 <= 5` | `False` |

Podemos usar a função `print()` para exibir o resultado das comparações:

```python
print(10 == 10)    # True: os valores são iguais
print(5 != 3)      # True: os valores são diferentes
print(7 > 2)       # True: 7 é maior que 2
print(4 < 1)       # False: 4 não é menor que 1
print(8 >= 8)      # True: 8 é maior ou igual a 8
print(3 <= 2)      # False: 3 não é menor ou igual a 2
```

### Comparações entre variáveis

- Podemos realizar comparações entre variáveis.

```python 
a = 5
b = 10

print(a == b)   # False: 5 não é igual a 10
print(a != b)   # True: 5 é diferente de 10
print(a < b)    # True: 5 é menor que 10
print(a > b)    # False: 5 não é maior que 10
```
- Python também permite comparar números com variáveis e expressões.

```python
x = 3
y = 3.0

print(x == y)             # True: 3 (int) é igual a 3.0 (float)
print(type(x) == type(y)) # False: os tipos são diferentes
```

É possível comparar strings (texto).

```python
print("casa" == "casa")      # True
print("casa" != "Casa")      # True: Python diferencia maiúsculas e minúsculas
print("abacate" < "banana")  # True: ordem alfabética
```
