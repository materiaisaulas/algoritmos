#### Set (`set`)

O **`set`** é uma estrutura de dados em Python utilizada para armazenar **múltiplos valores em uma única variável**.

A principal característica de um `set` é que **ele não permite elementos repetidos**. Se um mesmo valor for inserido mais de uma vez, apenas **uma ocorrência será mantida**.

Além disso, os elementos de um `set` **não possuem uma ordem fixa**, portanto os valores podem aparecer em qualquer ordem quando exibidos.


#### Criando um set

Um `set` pode ser criado utilizando **chaves `{}`** ou a função **`set()`**.

```python
numeros = {10, 20, 30, 40}
````

Também é possível criar um `set` a partir de outra coleção, como uma lista.

```python
numeros = set([10, 20, 30, 40])
```

Nesse caso, a lista é convertida para um `set`.

Se valores repetidos forem informados durante a criação do `set`, eles **não serão armazenados mais de uma vez**.

```python
numeros = {10, 20, 20, 30, 30, 40}
print(numeros)
```

Saída:

```
{10, 20, 30, 40}
```

Observe que os valores duplicados **foram automaticamente eliminados**.

### Adicionando elementos

Para inserir um novo elemento em um `set`, utilizamos o método **`add()`**.

```python
numeros = {10, 20, 30}
numeros.add(40)
print(numeros)
```

#### Removendo elementos

Para remover um elemento, utilizamos o método **`remove()`**.

```python
numeros = {10, 20, 30, 40}
numeros.remove(20)
print(numeros)
```

#### Percorrendo um set

Também podemos percorrer os elementos de um `set` utilizando um laço `for`.

```python
numeros = {10, 20, 30, 40}
for numero in numeros:
    print(numero)
```

Como os elementos não possuem ordem definida, eles podem aparecer **em qualquer sequência**.


#### Aplicação prática: removendo valores repetidos

Uma aplicação muito comum do `set` é **eliminar valores duplicados de uma lista**.

```python
numeros = [10, 20, 20, 30, 30, 40]
numeros_sem_repeticao = set(numeros)
print(numeros_sem_repeticao)
```

Saída:

```
{10, 20, 30, 40}
```

Nesse exemplo, a lista foi convertida para um `set`, removendo automaticamente os valores repetidos.


Outra situação comum é verificar se determinado valor **faz parte de um conjunto de elementos**. Para isso utilizamos o operador **`in`**, que permite testar se um elemento pertence a um `set`.


```python
cores_permitidas = {"vermelho", "azul", "verde"}

cor = "azul"

if cor in cores_permitidas:
    print("Cor permitida")
else:
    print("Cor não permitida")
````

Saída:

```
Cor permitida
```

Nesse exemplo, o programa verifica se a variável `cor` está presente no conjunto `cores_permitidas`.
Se o valor estiver no `set`, a condição é verdadeira e a mensagem **"Cor permitida"** é exibida.



