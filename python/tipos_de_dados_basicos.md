### Tipos de dados básicos

Todo programa trabalha com dados, e o Python oferece tipos básicos que cobrem a maioria das situações iniciais. Os principais são:

Inteiros (int) - São números inteiros, positivos ou negativos, sem parte decimal.

```python
idade = 25
ano = 2025
temperatura_negativa = -5
```

Esses valores podem ser usados diretamente em operações aritméticas:

```python
soma = 10 + 5
print(soma)  # saída: 15
```

Ponto flutuante (float)
São números que possuem parte decimal. Use ponto (.) como separador decimal.

```python
altura = 1.75
preco = 9.99
desconto = -0.2
```

Floats também podem participar de operações matemáticas:

```python
media = (7.5 + 8.0 + 6.0) / 3
print(media)  # saída: 7.166666666666667
```

Strings (str) - São sequências de caracteres, usadas para representar texto. Devem ser envolvidas por aspas simples (') ou duplas ("):

```python
nome = "Ana"
mensagem = 'Olá, mundo!'
Strings podem ser concatenadas e manipuladas:
saudacao = "Olá, " + nome
print(saudacao)  # saída: Olá, Ana
```
Booleanos (bool) - Representam valores lógicos: True (verdadeiro) ou False (falso). São usados com operadores de comparação ou lógicos.

```python
ligado = True
desligado = False
```

É possível obter booleanos a partir de comparações:

```python 
maior_de_idade = idade >= 18
print(maior_de_idade)  # saída: True
```

Explorando no VS Code - Você pode testar esses exemplos diretamente em um novo arquivo .py, por exemplo:

```python 
# tipos_basicos.py
nome = "José"
idade = 42
altura = 1.80
tem_carteira = True

print("Nome:", nome)
print("Idade:", idade)
print("Altura:", altura)
print("Possui carteira de motorista?", tem_carteira)
```

:::definition Tipos de dados imutáveis

Em Python, um **tipo de dado imutável** é aquele cujo valor **não pode ser alterado após a sua criação**. Isso significa que, depois que um objeto é criado, seu conteúdo permanece o mesmo durante toda a execução do programa.

Se for necessário trabalhar com um valor diferente, na prática o Python cria **um novo valor**, em vez de modificar o valor existente.

Alguns exemplos de tipos de dados imutáveis em Python são:

- **inteiros (`int`)**
- **números de ponto flutuante (`float`)**
- **strings (`str`)**

Exemplo:

```python
numero = 10
texto = "Python"

:::