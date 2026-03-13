### Entrada e saída

Na programação, entrada e saída de dados são elementos fundamentais para a interação entre o usuário e o programa. Em Python, esses processos são realizados principalmente com as funções input() e print(). A entrada de dados permite que o usuário forneça informações ao programa em tempo de execução, enquanto a saída de dados exibe mensagens, resultados de cálculos ou qualquer outro tipo de informação.

A função input() lê dados do teclado como texto (string), e frequentemente é usada em conjunto com conversões de tipo, quando precisamos que o dado seja tratado como número (int, float, etc.). Já a função print() é utilizada para mostrar informações no console, sendo uma das primeiras formas de verificar se um programa está funcionando corretamente.

Um recurso muito útil, especialmente ao exibir mensagens personalizadas, é a formatação de strings. Com ela, podemos combinar texto fixo com valores de variáveis de forma clara e elegante. Python oferece diferentes formas de fazer isso, sendo as mais modernas e recomendadas as chamadas f-strings, que permitem incorporar variáveis diretamente no texto.

Assim, ao combinar entrada, saída e formatação de strings, criamos programas mais interativos, compreensíveis e fáceis de usar. Esses conceitos são essenciais desde os primeiros passos na programação e continuam sendo úteis mesmo em aplicações mais avançadas.


Em qualquer linguagem de programação, a entrada de dados é a maneira como um programa coleta informações do usuário, e a saída de dados é a forma como ele retorna essas informações ou resultados. Em Python, essas ações são bastante simples e diretas.

Entrada de dados com input()

A função input() permite que o usuário digite algo no console. Ela sempre retorna uma string, mesmo que o usuário digite um número.

Neste exemplo, usamos int() para converter a entrada de string para inteiro. Também poderíamos usar float() para números com casas decimais.

:::example
```python 
nome = input("Digite seu nome: ")
print("Olá,", nome)
```

Se quisermos tratar o valor como número, é necessário converter:

```python
idade = int(input("Digite sua idade: "))
print("Você tem", idade, "anos")
```
:::

Saída de dados com print()

A função print() é usada para exibir mensagens ou resultados no console. Ela pode concatenar textos, mostrar variáveis e até expressões.

:::example
```python 
print("A soma de 2 + 3 é", 2 + 3)
```
Também é possível usar f-strings, que tornam a escrita mais legível:

```python
nome = "Maria"
idade = 30
print(f"{nome} tem {idade} anos.")
```

Para que o programa não dependa de um ano fixo, o ideal é obter o ano atual diretamente do sistema operacional. Em Python isso pode ser feito utilizando o módulo datetime.

Primeiro é importado o módulo `from datetime import datetime`, que permite acessar informações de data e hora do sistema operacional. Em seguida, o programa solicita ao usuário o nome e o ano de nascimento. A instrução `datetime.now()`.year captura o ano atual do computador onde o programa está sendo executado. Depois disso, o programa calcula a idade subtraindo o ano de nascimento do ano atual. Por fim, o resultado é exibido na tela com uma mensagem personalizada para o usuário.

```python 
from datetime import datetime

nome = input("Qual é o seu nome? ")
ano_nascimento = int(input("Em que ano você nasceu? "))
ano_atual = datetime.now().year
idade = ano_atual - ano_nascimento
print(f"Olá, {nome}! Você tem {idade} anos em {ano_atual}.")
```
:::
​