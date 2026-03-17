### Tuplas (`tuple`)

As **tuplas** são uma coleção utilizada para armazenar **múltiplos valores em uma única variável**, de forma semelhante às listas.

A principal diferença é que as **tuplas são imutáveis**, ou seja, **seus elementos não podem ser alterados após a criação**.

Isso significa que, depois de criada, uma tupla **não permite adicionar, remover ou modificar elementos**.

Uma tupla é criada utilizando **parênteses `()`** e separando os elementos por vírgula.

```python
numeros = (10, 20, 30, 40)
````

Nesse exemplo, a variável `numeros` armazena quatro valores organizados em sequência.

Assim como nas listas, cada elemento possui um **índice**, que começa em **0**.

| Índice | 0| 1| 2| 3|
|--------|--|--|--|--|
| Valor  |10|20|30|40|


### Acessando elementos

Os elementos de uma tupla podem ser acessados utilizando **seu índice**, da mesma forma que nas listas.

```python
numeros = (10, 20, 30, 40)

print(numeros[0])
print(numeros[2])
```

Saída esperada:

```
10
30
```

De forma análoga a listas, é possível percorrer seus elementos utilizando estruturas de repetição.

:::compare usando for while para percorrer tuplas

```python
numeros = (10, 20, 30, 40)

for numero in numeros:
    print(numero)
```

---

```python
numeros = (10, 20, 30, 40)

indice = 0

while indice < len(numeros):
    print(numeros[indice])
    indice += 1
```

---

O laço **`for`** percorre diretamente os elementos da tupla, já o **`while`** exige o controle manual do índice e utiliza a função `len()` para limitar a repetição.

:::


:::info
Como as tuplas são **imutáveis**, não é possível realizar operações como:

* adicionar elementos
* remover elementos
* alterar valores por índice

Por exemplo, o código abaixo gera erro:

```python
numeros = (10, 20, 30)
numeros[1] = 99
```

Isso ocorre porque **tuplas não permitem alteração de seus elementos após a criação**.
:::

### Quando utilizar tuplas

As tuplas são utilizadas quando precisamos armazenar **um conjunto de valores que não deve ser alterado durante a execução do programa**.

Como as tuplas são **imutáveis**, elas ajudam a garantir que determinados dados permaneçam constantes.

Alguns exemplos comuns de uso são:

- **coordenadas** de um ponto (x, y)
- **dados fixos** como dias da semana
- **valores que representam uma posição ou configuração**

:::example
coordenadas de um ponto

```python
ponto = (10, 20)
print(ponto[0])
print(ponto[1])

````

Nesse caso, a tupla representa a posição de um ponto no plano cartesiano.

dias da semana

```python
dias_semana = ("segunda", "terça", "quarta", "quinta", "sexta", "sábado", "domingo")
print(dias_semana[0])

```

Como os dias da semana **não mudam**, faz sentido armazená-los em uma **tupla**.

:::

:::note Para lembrar
Na prática, **listas são utilizadas quando os dados podem mudar**, enquanto **tuplas são usadas quando os dados devem permanecer constantes**.
:::



