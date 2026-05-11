# Tipos de Dados

## o que sao tipos de dados?

Servem para definir as caracteristicas de um valor, ou seja, o tipo de dado define o tipo de valor que uma variável pode armazenar e quantos bytes de memória são necessários para armazenar esse valor.

## tipos de dados em python

### tipos de dados que eu ja testei

- int: números inteiros, como 1, 2, 3, etc.
- float: números decimais, como 3.14, 2.5,
- str: strings, ou seja, sequências de caracteres, como "Olá", "Python", etc.
- bool: valores booleanos, que podem ser True ou False.

### tipos ainda estranhos pra mim

- list: listas, que são coleções ordenadas de valores, como [1, 2, 3], ["a", "b", "c"], etc.
- tuple: tuplas, que são coleções ordenadas e imutáveis de valores,
- dict: dicionários, que são coleções de pares chave-valor, como {"nome": "João", "idade": 30}, etc.
- set: conjuntos, que são coleções de valores únicos e não ordenados, como {1, 2, 3}, {"a", "b", "c"}, etc.
- NoneType: tipo de dado que representa a ausência de valor, ou seja, quando uma variável não tem um valor atribuído, ela é do tipo NoneType e tem o valor None.
- complex: números complexos, que são compostos por uma parte real e uma parte imaginária, como 2 + 3j, etc.
- bytes: tipo de dado que representa uma sequência de bytes, usado para armazenar dados binários, como arquivos, imagens, etc.
- bytearray: tipo de dado que representa uma sequência mutável de bytes, usado para armazenar dados binários que podem ser modificados, como arquivos, imagens, etc.
- frozenset: tipo de dado que representa um conjunto imutável de valores únicos e não ordenados, como frozenset({1, 2, 3}), frozenset({"a", "b", "c"}), etc.
- range: tipo de dado que representa uma sequência de números inteiros, usado para criar loops e iterar sobre sequências de números, como range(0, 10), range(1, 5), etc.
- memoryview: tipo de dado que representa uma visão de memória, usado para acessar e manipular dados binários sem copiar os dados para a memória, como memoryview(b"Hello"), etc.
- None: tipo de dado que representa a ausência de valor, ou seja, quando uma variável não tem um valor atribuído, ela é do tipo NoneType e tem o valor None.
- ellipsis: tipo de dado que representa um valor de elipse, usado para indicar que um valor é omitido ou desconhecido, como ... (três pontos), etc.
- NotImplemented: tipo de dado que representa um valor que indica que uma operação ou método não é implementado, usado para indicar que uma operação ou método não é suportado por um objeto, como NotImplemented, etc.
- type: tipo de dado que representa o tipo de um objeto, usado para verificar o tipo de um objeto em tempo de execução, como type(1), type("Hello"), etc.
- object: tipo de dado que representa o tipo base de todos os objetos em Python, usado para criar classes e objetos personalizados, como object(), etc.


# tipo int

int é um objeto que representa um número inteiro, ou seja, um número sem parte decimal. Ele pode ser positivo, negativo ou zero. O tipo int é usado para armazenar valores inteiros e realizar operações matemáticas com esses valores.

# tipo float

float é um objeto que representa um número decimal, ou seja, um número com parte decimal. Ele pode ser positivo, negativo ou zero. O tipo float é usado para armazenar valores decimais e realizar operações matemáticas com esses valores.

# tipo str

str é um objeto que representa uma sequência de caracteres, ou seja, um texto. Ele pode conter letras, números, símbolos e espaços. O tipo str é usado para armazenar valores de texto e realizar operações com esses valores, como concatenar strings, acessar caracteres individuais, etc.

Contantes str podem ser representadas usando aspas simples (' '), aspas duplas (" ") ou aspas triplas (''' ''' ou """ """). As aspas triplas são usadas para criar strings multilinha, ou seja, strings que ocupam mais de uma linha.

# tipo bool

bool é um objeto que representa um valor booleano, ou seja, um valor que pode ser verdadeiro (True) ou falso (False). O tipo bool é usado para armazenar valores booleanos e realizar operações lógicas com esses valores, como comparações, operadores lógicos, etc.

o objeto bool é uma subclasse do tipo int, o que significa que os valores True e False são equivalentes a 1 e 0, respectivamente. Isso permite que os valores booleanos sejam usados em operações matemáticas e lógicas, como somar True + True para obter 2, ou usar False em uma expressão condicional para indicar que a condição é falsa.

