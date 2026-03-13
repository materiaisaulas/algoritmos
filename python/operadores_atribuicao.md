### Operadores de atribuição 

Em Python, operadores de atribuição são utilizados para armazenar valores em variáveis. O mais comum é o operador =, que simplesmente atribui o valor do lado direito à variável do lado esquerdo. No entanto, há diversos operadores de atribuição compostos que realizam uma operação matemática e já atualizam a variável com o novo valor. Esses operadores ajudam a escrever o código de forma mais compacta e eficiente.

Esses operadores são úteis quando você precisa atualizar o valor de uma variável com base nela mesma. Por exemplo, em contadores, acumuladores ou ao aplicar fórmulas matemáticas. Eles também melhoram a legibilidade do código, deixando claro que a variável está sendo modificada com base em seu valor atual.

| Operação | Equivalente | Descrição |
|----------|-------------|-----------|
| `x = 10` | `x = 10` | Atribuição simples: a variável `x` recebe o valor 10 |
| `x += 5` | `x = x + 5` | Soma 5 ao valor atual de `x` |
| `x -= 2` | `x = x - 2` | Subtrai 2 do valor atual de `x` |
| `x *= 3` | `x = x * 3` | Multiplica o valor de `x` por 3 |
| `x /= 2` | `x = x / 2` | Divide o valor de `x` por 2 |
| `x %= 3` | `x = x % 3` | Calcula o resto da divisão de `x` por 3 |
| `x **= 2` | `x = x ** 2` | Eleva `x` ao quadrado (potência) |
| `x //= 4` | `x=x//(x//4)` | Realiza divisão inteira de `x` por 4 |


:::example
Neste exemplo ocorre uma **atribuição simples**. A variável `x` passa a armazenar o valor `10`. Em programação, o operador `=` não representa igualdade matemática, mas sim **atribuição de valor a uma variável**. Após a execução da instrução, quando o comando `print(x)` é executado, o programa exibe o valor armazenado em `x`, que é `10`.

```python
x = 10
print(x)
```

O operador `+=` é um **operador de atribuição com soma**. Ele soma um valor ao conteúdo atual da variável. Nesse exemplo, a variável `x` começa com o valor `10`. Ao executar `x += 5`, o valor `5` é somado ao valor atual de `x`. Assim, o novo valor armazenado na variável passa a ser `15`.

```python
x = 10
x += 5
print(x)
```

O operador `-=` realiza uma **subtração seguida de atribuição**. Isso significa que o valor indicado será subtraído do valor atual da variável. No exemplo, `x` inicia com `10`. Ao executar `x -= 2`, o programa calcula `10 - 2`, armazenando o resultado `8` em `x`.

```python
x = 10
x -= 2
print(x)
```

O operador `*=` realiza uma **multiplicação seguida de atribuição**. Nesse caso, o valor atual da variável é multiplicado pelo valor indicado. Como `x` começa valendo `10`, ao executar `x *= 3`, o programa calcula `10 × 3`, resultando em `30`, que passa a ser o novo valor da variável.

```python
x = 10
x *= 3
print(x)
```

O operador `/=` realiza uma **divisão seguida de atribuição**. O valor atual da variável é dividido pelo número indicado. No exemplo, `x` começa com `10`. Ao executar `x /= 2`, o programa calcula `10 ÷ 2`, resultando em `5.0`. Em Python, a divisão com `/` produz um resultado do tipo **float**, mesmo quando a divisão é exata.

```python
x = 10
x /= 2
print(x)
```

O operador `%=` utiliza o **operador módulo**, que calcula o **resto da divisão inteira**. Nesse exemplo, `x` começa com `10`. Quando executamos `x %= 3`, o programa calcula o resto da divisão de `10` por `3`. Como `3 × 3 = 9` e sobra `1`, o valor armazenado em `x` passa a ser `1`.


```python
x = 10
x %= 3
print(x)
```

O operador `**=` realiza uma **operação de potência seguida de atribuição**. Isso significa que o valor da variável é elevado à potência indicada. No exemplo, `x` inicia com `5`. Ao executar `x **= 2`, o programa calcula `5²`, resultando em `25`. Assim, `x` passa a armazenar o valor `25`.

```python
x = 5
x **= 2
print(x)
```

O operador `//=` realiza uma **divisão inteira seguida de atribuição**. A divisão inteira descarta a parte decimal do resultado. No exemplo, `x` começa com `10`. Ao executar `x //= 4`, o programa calcula `10 // 4`. O resultado da divisão inteira é `2`, pois `4` cabe duas vezes em `10`, ignorando o restante da divisão.


```python
x = 10
x //= 4
print(x)
```
:::