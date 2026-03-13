### Desvios em Estruturas de Repetição

Em algumas situações, durante a execução de um laço de repetição, pode ser necessário **interromper a repetição antes do previsto** ou **pular parte do código dentro do laço**.

Para esses casos, Python possui algumas instruções chamadas **desvios de controle**, que modificam o comportamento normal da repetição.

As principais são:

* `break`
* `continue`
* `pass`

Essas instruções podem ser utilizadas tanto em **laços `for` quanto em `while`**.

### O comando `break`

O comando **`break`** é utilizado para **interromper imediatamente a execução do laço**, mesmo que ainda existam valores na sequência ou que a condição do `while` ainda seja verdadeira.

Quando o `break` é executado, o Python **sai do laço e continua a execução do programa nas instruções seguintes**.

### Exemplo com `for`

:::example


```python
for i in range(10):
    
    if i == 5:
        break
    
    print(i)
```

Saída:

```
0
1
2
3
4
```
Nesse exemplo, o laço foi programado para contar até **9**, mas quando `i` assume o valor **5**, o comando `break` é executado e o laço é encerrado imediatamente.
:::


### Exemplo com `while`

:::example


```python
i = 0
while True:   
    if i == 5:
        break
    print(i)
    i = i + 1
```

Saída:

```
0
1
2
3
4
```

Nesse caso, o laço foi criado com `while True`, que geraria uma repetição infinita. No entanto, o comando `break` é utilizado para **encerrar o laço quando a condição desejada é atingida**.
:::

### O comando `continue`

O comando **`continue`** não interrompe o laço.
Ele apenas **faz o Python pular para a próxima repetição**, ignorando o restante das instruções daquele ciclo.

:::example

```python
for i in range(6):
    
    if i == 3:
        continue
    
    print(i)
```

Saída:

```
0
1
2
4
5
```

Observe que o número **3 não foi exibido**. Quando `i` assume o valor 3, o comando `continue` é executado e o Python **passa diretamente para a próxima repetição**, sem executar o `print`.

:::


### O comando `pass`

O comando `pass` é uma instrução que não executa nenhuma ação. Diferentemente de `break` e `continue`, ele não altera o fluxo de execução do laço.

Sua função é apenas manter a estrutura sintática do programa válida, ocupando o lugar onde uma instrução poderia existir.

Em Python, algumas estruturas — como `if`, `for`, `while`, funções ou classes — exigem que exista pelo menos uma instrução dentro do bloco. Quando ainda não desejamos implementar nenhuma ação naquele ponto do programa, podemos utilizar o `pass`.


:::example

```python
for i in range(5):
    
    if i == 2:
        pass
    
    print(i)
```

Saída:

```
0
1
2
3
4
```

Nesse exemplo, o `pass` **não altera o comportamento do programa**. Ele apenas indica que **nenhuma ação será executada naquele bloco**.
Esse comando é frequentemente utilizado **durante o desenvolvimento do código**, quando uma parte do programa ainda será implementada posteriormente.
:::

Podemos resumir o comportamento dessas instruções da seguinte forma:

| Comando    | Comportamento                  |
| ---------- | ------------------------------ |
| `break`    | encerra o laço imediatamente   |
| `continue` | pula para a próxima repetição  |
| `pass`     | não faz nada (instrução vazia) |

---

> Assim como ocorre com os laços `for` e `while`, essas instruções são executadas **de forma sequencial pelo interpretador**. Quando um desvio é encontrado, o fluxo de execução é alterado, permitindo interromper ou modificar o comportamento da repetição de maneira controlada.
