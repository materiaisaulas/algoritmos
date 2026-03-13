### Listas (`list`)

Entre as coleções disponíveis em Python, a **lista (`list`)** é uma das mais utilizadas.

Uma **lista** é uma estrutura que permite armazenar **vários valores em uma única variável**, mantendo esses valores **organizados em uma sequência**. Cada elemento da lista ocupa uma posição chamada **índice**, que começa em **0**. As listas são **mutáveis**, ou seja, seus elementos podem ser alterados após a criação.

Em Python, uma lista é criada utilizando **colchetes `[]`** e separando os elementos por vírgula.

```python
numeros = [10, 20, 30, 40, 50]
```

Nesse exemplo, a variável `numeros` armazena cinco valores organizados em sequência.

| Índice | 0| 1| 2| 3| 4|
|--------|--|--|--|--|--|
| Valor  |10|20|30|40|50|

Podemos acessar qualquer elemento da lista utilizando seu **índice**.

```python
print(numeros[0])  # 10
print(numeros[2])  # 30
```

Uma tarefa muito comum é **percorrer todos os elementos de uma lista**, realizando alguma operação com cada valor. Isso pode ser feito utilizando estruturas de repetição como **`for`** e **`while`**.

:::compare Percorrendo uma lista com `for` e `while`

```python
numeros = [10, 20, 30, 40, 50]
for numero in numeros:
    print(numero)
```

---

```python
numeros = [10, 20, 30, 40, 50]
indice = 0
while indice < len(numeros):
    print(numeros[indice])
    indice += 1
```

---

O laço **`for`** percorre diretamente os elementos da lista, tornando o código mais simples e legível.
Já o **`while`** exige o controle manual do índice da lista, utilizando uma variável de controle e a função `len()` para limitar a repetição.



:::


:::info

Quando o objetivo é **percorrer todos os elementos de uma coleção**, o **`for` costuma ser a forma mais simples e recomendada** em Python.

O **`while`** é mais utilizado quando a repetição depende de **uma condição específica**, e não apenas da quantidade de elementos de uma sequência.

:::

### Operações básicas com listas

Depois de criar uma lista, é comum realizar operações como **adicionar**, **remover** ou **consultar** elementos. Essas operações permitem modificar o conteúdo da lista ao longo da execução do programa.

Para adicionar um novo elemento ao final da lista, utilizamos o método **`append()`**, que insere um novo elemento sempre na última posição da lista. 

```python
numeros = [10, 20, 30]
numeros.append(40)
print(numeros)
```

Saída:

```
[10, 20, 30, 40]
```

Para remover um elemento específico da lista, podemos utilizar o método **`remove()`**.

```python
numeros = [10, 20, 30, 40]

numeros.remove(20)

print(numeros)
```

Saída:

```
[10, 30, 40]
```

Nesse caso, o valor **20** foi removido da lista.

A função **`len()`** retorna a quantidade de elementos existentes na lista. Essa função é muito utilizada em **estruturas de repetição**, especialmente em laços `while`.

```python
numeros = [10, 20, 30, 40, 50]

print(len(numeros))
```

Saída:

```
5
```

Como as listas são **mutáveis**, é possível modificar diretamente um elemento utilizando seu índice.

```python
numeros = [10, 20, 30]

numeros[1] = 99

print(numeros)
```

Saída:

```
[10, 99, 30]
```

Nesse exemplo, o valor **20** foi substituído por **99**.

Um **resumo visual simples** funciona bem na apostila porque permite ao aluno **revisar rapidamente as operações mais usadas** com listas.

A tabela abaixo mantém apenas **os elementos essenciais**: operação, exemplo e resultado.

---

### Resumo das operações básicas com listas

| Operação           | Exemplo                  | Resultado                         |
| ------------------ | ------------------------ | --------------------------------- |
| Criar lista        | `numeros = [10, 20, 30]` | cria uma lista com três elementos |
| Acessar elemento   | `numeros[1]`             | retorna `20`                      |
| Alterar elemento   | `numeros[1] = 99`        | `[10, 99, 30]`                    |
| Adicionar elemento | `numeros.append(40)`     | `[10, 20, 30, 40]`                |
| Remover elemento   | `numeros.remove(20)`     | `[10, 30]`                        |
| Tamanho da lista   | `len(numeros)`           | quantidade de elementos           |



### Listas com `if`

Quando trabalhamos com listas, é comum verificar **condições relacionadas aos elementos armazenados**. Para isso, utilizamos **estruturas condicionais**, como o comando `if`. Uma situação típica é **percorrer a lista e verificar alguma característica dos elementos**, como identificar números maiores que um determinado valor. Um exemplo simples é verificar maiores que 10 

```python
numeros = [5, 12, 8, 20, 3, 15]
for numero in numeros:
    if numero > 10:
        print(numero)
```

Saída:

```
12
20
15
```

Nesse exemplo:

* a lista `numeros` possui vários valores
* o laço `for` percorre cada elemento da lista
* o `if` verifica se o valor é **maior que 10**
* apenas os valores que atendem à condição são exibidos

Identificando números pares, onde é possível utilizar operadores como o **módulo (`%`)** para verificar propriedades numéricas.

```python
numeros = [3, 6, 9, 12, 15, 18]
for numero in numeros:
    if numero % 2 == 0:
        print(numero)
```

Saída:

```
6
12
18
```

Nesse caso:

* `numero % 2` calcula o **resto da divisão por 2**
* se o resto for **0**, o número é **par**

---

Verificando se um valor existe na lista. Também podemos utilizar o operador **`in`** para verificar se um elemento está presente na lista.

```python
numeros = [10, 20, 30, 40]
if 20 in numeros:
    print("O valor está na lista")
```

Saída:

```
O valor está na lista
```

### Listas dentro de listas

Uma lista pode armazenar qualquer tipo de valor, inclusive **outras listas**. Quando isso acontece, temos uma **lista de listas**. Essa estrutura é útil quando precisamos organizar dados em **linhas e colunas**, de forma semelhante a uma tabela.

Exemplo de lista dentro de lista

```python
notas = [
    [7, 8, 9],
    [6, 5, 7],
    [9, 8, 10]
]

print(notas)
```

Nesse exemplo, a variável `notas` contém **três listas internas**, cada uma representando um conjunto de valores.

Podemos imaginar essa estrutura como uma tabela:

| Linha | Valores    |
| ----- | ---------- |
| 0     | [7, 8, 9]  |
| 1     | [6, 5, 7]  |
| 2     | [9, 8, 10] |


Para acessar um valor específico, utilizamos **dois índices**:

* o primeiro indica a **lista principal**
* o segundo indica o **elemento dentro da lista interna**

```python
print(notas[0][1])
```

Saída:

```
8
```

Nesse caso:

* `notas[0]` acessa a primeira lista `[7, 8, 9]`
* `[1]` acessa o segundo elemento dessa lista


Também podemos percorrer essas estruturas utilizando **laços de repetição**.

```python
notas = [
    [7, 8, 9],
    [6, 5, 7],
    [9, 8, 10]
]

for linha in notas:
    for valor in linha:
        print(valor)
```

Esse código percorre **cada lista interna** e depois **cada valor dentro dela**.

Podemos utilizar listas dentro de listas para representar **notas de alunos**.

```python
notas = [
    [7, 8, 9],
    [6, 5, 7],
    [9, 8, 10]
]

for aluno in notas:
    media = sum(aluno) / len(aluno)
    print(media)
```

Nesse exemplo:

* cada lista representa as **notas de um aluno**
* a função **`sum()`** recebe como parâmetro **uma sequência de números**, como uma lista. Esse parâmetro indica quais valores devem ser somados. No exemplo `sum(aluno)`, a lista `aluno` é passada para a função, que soma todos os números presentes nela e retorna o resultado dessa soma.
* `len()` indica a quantidade de notas
* o programa calcula a **média de cada aluno**


Listas dentro de listas são frequentemente usadas para representar:

* **tabelas de dados**
* **planilhas**
* **matrizes matemáticas**
* **estruturas organizadas em linhas e colunas**

Esse conceito aparece em muitas aplicações, como **análise de dados, jogos, planilhas e algoritmos científicos**.

