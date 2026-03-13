Em Python, os principais operadores lógicos são:

```bash
and (E lógico)
or (OU lógico)
not (NÃO lógico)
```
Esses operadores são usados para combinar ou inverter valores booleanos. Vamos ver cada um com exemplos e explicações.


:::example

- and – Conjunção lógica (E)
- Retorna True se ambos os lados forem True.

```
print(True and True)   # True
print(True and False)  # False
print(False and False) # False
```

- Leitura: "Verdadeiro e verdadeiro é verdadeiro", mas "verdadeiro e falso é falso".

:::

:::example

- or – Disjunção lógica (OU)
- Retorna True se pelo menos um dos lados for True.
```
print(True or True)    # True
print(True or False)   # True
print(False or False)  # False
```
- Leitura: "Verdadeiro ou falso é verdadeiro", pois só um dos lados precisa ser True.
:::

:::example

- not – Negação lógica (NÃO)
- Inverte o valor lógico.
```
print(not True)   # False
print(not False)  # True
```
Leitura: "not True significa 'não verdadeiro', ou seja, False".
:::

Combinando operadores

Mesmo sem usar if, podemos brincar com combinações e ver os resultados:
```
print((5 > 3) and (2 < 4))     # True and True → True
print((10 == 2*5) or (1 > 5))  # True or False → True
print(not (7 <= 7))            # not True → False
```

Comparando variáveis numéricas

Aqui, a e b são inteiros. Usamos comparações (>, ==, <) combinadas com and, or e not.

```
a = 10
b = 5

print(a > b and b > 0)      # True and True → True
print(a == b or a < 20)     # False or True → True
print(not (a < b))          # not False → True

```

Comparando strings

Strings podem ser comparadas usando == (igual) e != (diferente), e os operadores lógicos funcionam da mesma forma.

```
nome = "Alice"
cidade = "São Paulo"

print(nome == "Alice" and cidade == "São Paulo")   # True and True → True
print(nome != "Bob" or cidade == "Rio")            # True or False → True
print(not (cidade == "Rio"))                       # not False → True
````

Misturando tipos — números e booleanos

Note que maior_de_idade já é uma variável booleana, e pode ser usada diretamente com operadores lógicos.

```
idade = 20
maior_de_idade = idade >= 18

print(maior_de_idade and idade < 30)  # True and True → True
print(idade < 18 or maior_de_idade)   # False or True → True
print(not maior_de_idade)            # not True → False
```

Expressões com variáveis booleanas e strings

Mesmo que os tipos de variáveis sejam diferentes, os operadores lógicos funcionam normalmente desde que as expressões avaliem para True ou False.

```
ativo = True
usuario = "admin"

print(ativo and usuario == "admin")   # True and True → True
print(not ativo or usuario != "admin") # False or False → False
```





