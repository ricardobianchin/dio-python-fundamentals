# Funções de Entrada e Saída

## Função print()

A função print() é utilizada para exibir informações na tela. Ela pode receber um ou mais argumentos, que serão convertidos em string e exibidos.

O primeiro parametro é do tipo varargs, pode receber uma quantidade variável de argumentos.

print possui parâmetros opcionais, sep, end, file e flush, que permitem personalizar a saída.
- sep: define o separador entre os argumentos, o padrão é um espaço em branco
- end: define o que será impresso no final da linha, o padrão é uma nova linha
- file: define o destino da saída, o padrão é sys.stdout (a tela)
- flush: define se a saída deve ser forçada a ser escrita imediatamente, o padrão é False

Exemplo: 
``` python
print("Olá", "Mundo", sep="-", end="!\n") # Saída: Olá-Mundo! o \n equivale a quebra de linha
```

os valores default de sep e end são " " e "\n", respectivamente. Este comando:

```python
print("Olá", "Mundo") 
```

é equivalente a:

```python
print("Olá", "Mundo", sep=" ", end="\n")
```

Outro exemplo:
```python
nome = "Alice"
idade = 30

print("Nome:", nome, "Idade:", idade) # Saída: Nome: Alice  Idade: 30
print("Nome:", nome, "Idade:", idade, sep=" | ") # Saída: Nome: Alice | Idade: 30
print("Nome:", nome, "Idade:", idade, end=".\n") # Saída: Nome: Alice  Idade: 30.
print(f"Nome: {nome} | Idade: {idade}") # Saída: Nome: Alice | Idade: 30
```

## Função input()

A função input() é utilizada para ler uma entrada do usuário. Ela exibe uma mensagem opcional e aguarda o usuário digitar algo, retornando o valor digitado sempre como uma string.

Exemplo:

```python
nome = input("Digite seu nome: ") # O usuário digita "Alice" e a variável nome recebe o valor "Alice"
print("Olá, " + nome + "!") # Saída: Olá, Alice!
print(f"Olá, {nome}!") # Saída: Olá, Alice! utilizando f-string para interpolação de string
```
