# conversao de tipos

em alguns momentos é necessário converter um tipo de dado para outro para poder utilizá-lo

## conversão implícita

a conversão implícita é aquela feita automaticamente pelo interpretador do python, quando ele identifica que um tipo de dado pode ser convertido para outro sem perda de informação. 

exemplo:

```python
x = 10
y = 3.14
z = x + y
print(z) # 13.14
```

## conversão explícita

a conversão explícita é aquela feita pelo programador, utilizando as funções de conversão de tipos do python, como int(), float(), str(), etc.

## converter int para float

```python
x = 10
y = float(x)
print(y) # 10.0
```

## converter float para int

```python
x = 3.14
y = int(x)
print(y) # 3
```

## converter int para str

```python
x = 10
y = str(x)
print(y) # '10'

# ou

print(str(x)) # '10'

# ou

print(f'O valor de x é {x}') # 'O valor de x é 10'
```

## converter str para int

```python
x = '10'
y = int(x)
print(y) # 10
```

## converter str para float

```python
x = '3.14'
y = float(x)
print(y) # 3.14
```

## converter float para str

```python
pi = 3.14
pistr = str(pi)
print(pistr) # '3.14'
print(f'O valor de pi é {pi}') # 'O valor de pi é 3.14'
```
