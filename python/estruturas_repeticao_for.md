### Estruturas de Repetição

As estruturas de repetição, também chamadas de laços, permitem executar um bloco de código várias vezes de forma automática. Em Python, os dois principais tipos de repetição são `for` e `while`.

O laço **for** percorre uma sequência, como gerar, por exemplo, uma sequência de números. Ele é muito usado com a função range() para criar repetições controladas por contadores.


### Estrutura básica do `for`

```bash 
for variavel in sequencia:
    instruções
```

:::note A função range( inicio, fim, passo)

A função **`range()`**, que gera uma sequência de números inteiros, é muito utilizada em estruturas de repetição como o laço `for`, quando se deseja executar um bloco de código várias vezes. Essa função pode receber até três parâmetros: **início**, **fim** e **passo**. Quando usada com um único argumento, como `range(5)`, ela gera números começando em **0** e indo até **antes do valor informado** (0, 1, 2, 3 e 4). Quando são informados dois argumentos, como `range(2, 6)`, a sequência começa no **valor inicial** e vai até **antes do valor final** (2, 3, 4, 5). Já com três argumentos, como `range(0, 10, 2)`, além do início e do fim, define-se também o **intervalo entre os números gerados**, permitindo contagens de dois em dois, de três em três ou qualquer outro passo desejado, inclusive valores negativos para contagens decrescentes.

:::


A forma mais simples gera números **a partir de 0 até n−1**, isto é os números **0, 1, 2, 3 e 4**.

```python
for i in range(5):
    print("Contando: ", i)
```
Saída:

```
0
1
2
3
4
```

Podemos definir **de onde a contagem começa**, inicia em 1 e termina em 5 (6-1).

```python
for i in range(1, 6):
    print(i)
```

Saída:

```
1
2
3
4
5
```

Também podemos controlar **de quanto em quanto a contagem avança**, inicia em 0, termina em 9 (10-1) e avança de 2 em 2.

```python
for i in range(0, 10, 2):
    print(i)
```

Saída:

```
0
2
4
6
8
```

---

O `range()` também permite contagens decrescentes usando passo negativo, inicia em 10, termina em 1 (0-1), avança de -1 em -1.

```python
for i in range(10, 0, -1):
    print(i)
```

Saída:

```
10
9
8
7
6
5
4
3
2
1
```

Também é possível utilizar o `for` para percorrer outros tipos de sequência. Por exemplo, uma string que é uma sequência de caracteres, e o laço pode percorrer cada caractere individualmente.

```python 
for letra in "Python":
    print(letra)
```

Saída:
```
P
y
t
h
o
n
```

Nesse caso, a variável letra recebe cada caractere da palavra "Python" a cada repetição do laço.

> A ideia, portanto, é que você tenha compreendido o funcionamento do laço `for` de forma conceitual, observando como o interpretador executa a repetição. Inicialmente é gerada uma **sequência de valores** (por exemplo, por meio da função `range()`), e a variável de controle recebe o **primeiro valor dessa sequência**. Em seguida, o bloco de instruções dentro do laço é executado. Após essa execução, a variável recebe **o próximo valor da sequência**, e o bloco é executado novamente. Esse processo se repete sucessivamente até que **todos os valores da sequência tenham sido utilizados**, momento em que o laço é encerrado e a execução do programa continua nas instruções seguintes.

