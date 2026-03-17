### Saída de dados

Na programação, **saída de dados** é o processo de apresentar informações ao usuário. Em Python, isso é feito principalmente por meio da função **`print()`**, que exibe mensagens e valores no console.

A função `print()` pode ser usada de diferentes maneiras, desde a exibição de textos simples até a apresentação de resultados de cálculos.

### Exibindo textos

A forma mais simples de usar `print()` é mostrar uma mensagem na tela.
```python 
print("Olá, mundo!")
print("Bem-vindo ao estudo de Python.")
```

Nesse caso, o programa apenas exibe mensagens escritas entre aspas.

### Exibindo valores de variáveis

Também podemos usar `print()` para mostrar valores armazenados em variáveis.
```python 
nome = "Maria"
idade = 30

print(nome)
print(idade)
```

Aqui o programa mostra o conteúdo das variáveis `nome` e `idade`.

### Exibindo resultados de expressões

A função `print()` também pode mostrar o resultado de cálculos ou expressões.
```python 
print("A soma de 2 + 3 é", 2 + 3)
print("O dobro de 10 é", 10 * 2)
```

Nesse exemplo, o Python calcula a expressão primeiro e depois exibe o resultado.


### Formatação de saída com f-strings

Uma forma moderna e mais legível de exibir informações é utilizando **f-strings**, que permitem inserir variáveis diretamente dentro do texto.
```python 
nome = "Maria"
idade = 30

print(f"{nome} tem {idade} anos.")
```

As chaves `{ }` indicam que o valor da variável será inserido dentro da mensagem.

:::note

Ao usar `print()`, podemos misturar **texto, variáveis e resultados de cálculos**, o que torna a saída do programa mais clara e informativa.
:::
