#### Dicionários (`dict`)

Os **dicionários** são uma coleção utilizada para armazenar **dados no formato chave–valor**.

Diferentemente de listas, tuplas e `set`, que armazenam apenas valores, os dicionários organizam os dados em **pares**, onde:

* a **chave** identifica a informação
* o **valor** representa o dado associado a essa chave

Essa estrutura é muito útil quando precisamos **associar um dado a um identificador**.

Um dicionário é criado utilizando **chaves `{}`**, onde cada elemento possui uma **chave e um valor separados por dois pontos (`:`)**.

```python
aluno = {
    "nome": "Ana",
    "idade": 20,
    "curso": "Engenharia"
}
```

Nesse exemplo:

| Chave | Valor      |
| ----- | ---------- |
| nome  | Ana        |
| idade | 20         |
| curso | Engenharia |


Para acessar um valor armazenado no dicionário, utilizamos **a chave correspondente**.

```python
aluno = {
    "nome": "Ana",
    "idade": 20,
    "curso": "Engenharia"
}

print(aluno["nome"])
print(aluno["idade"])
```

Saída esperada:

```
Ana
20
```

Podemos adicionar novos pares **chave–valor** ao dicionário.

```python
aluno = {
    "nome": "Ana",
    "idade": 20
}

aluno["curso"] = "Engenharia"

print(aluno)
```

Se a chave já existir, podemos **alterar o valor associado**.

```python
aluno = {
    "nome": "Ana",
    "idade": 20
}

aluno["idade"] = 21

print(aluno)
```

Para remover um elemento do dicionário, utilizamos o comando **`del`**.

```python
aluno = {
    "nome": "Ana",
    "idade": 20,
    "curso": "Engenharia"
}

del aluno["curso"]

print(aluno)
```

Também podemos percorrer os elementos de um dicionário utilizando um laço `for`.

```python
aluno = {
    "nome": "Ana",
    "idade": 20,
    "curso": "Engenharia"
}

for chave in aluno:
    print(chave, aluno[chave])
```

## Aplicação prática

Os dicionários são muito utilizados quando precisamos **organizar informações relacionadas**.

```python
produto = {
    "nome": "Notebook",
    "preco": 3500,
    "estoque": 12
}

print(produto["nome"])
print(produto["preco"])
```

Nesse exemplo, cada informação do produto é armazenada utilizando **uma chave que identifica o dado**.

#### Exemplo: registro de vários alunos

Podemos utilizar uma **lista de dicionários** para armazenar os dados de vários alunos.

Cada dicionário representa **um aluno**, enquanto a lista agrupa todos os registros.

```python
alunos = [
    {
        "nome": "Ana",
        "idade": 20,
        "curso": "Engenharia",
        "media": 8.7
    },
    {
        "nome": "Carlos",
        "idade": 22,
        "curso": "Computação",
        "media": 7.9
    },
    {
        "nome": "Mariana",
        "idade": 21,
        "curso": "Arquitetura",
        "media": 9.1
    }
]

for aluno in alunos:
    print(aluno["nome"], aluno["media"])
````

Saída possível:

```
Ana 8.7
Carlos 7.9
Mariana 9.1
```

Nesse exemplo:

* cada **dicionário** representa um aluno
* a **lista** armazena todos os alunos
* o laço `for` percorre os registros e exibe algumas informações


:::note Quando utilizar dicionários

Os dicionários são indicados quando precisamos:
* associar **informações a identificadores**
* representar **registros de dados**
* organizar **informações estruturadas**

Exemplos comuns incluem:
* dados de alunos
* informações de produtos
* configurações de sistemas
* registros de usuários

:::