# Manipulando listas

## Declarando uma lista de cavaleiros
```python
cavaleiros = ['Seya', 'Aldebaran', 'Aldebaran', 'Shun', 'Shiryu', 'Yoga']

print(cavaleiros)
```
### Resultado
`['Seya', 'Aldebaran', 'Aldebaran', 'Shun', 'Shiryu', 'Yoga']`

## adiciona um novo elemento ao final da lista

```python
cavaleiros.append('Ikki')
print(cavaleiros)
```
### Resultado
`['Seya', 'Aldebaran', 'Aldebaran', 'Shun', 'Shiryu', 'Yoga', 'Ikki']`

## extendendo a lista com outra lista

```python
cavaleiros.extend(['Shina', 'Maryn'])
print(cavaleiros)
```
### Resultado
`['Athena', 'Seya', 'Aldebaran', 'Aldebaran', 'Shun', 'Shiryu', 'Yoga', 'Ikki', 'Shina', 'Maryn']`

 ## inserir na lista em uma posição especifica
 
 ```python
cavaleiros.insert(0, 'Athena')
print(cavaleiros)
``` 
### Resultado
`['Athena', 'Seya', 'Aldebaran', 'Aldebaran', 'Shun', 'Shiryu', 'Yoga', 'Ikki', 'Shina', 'Maryn']`

## remove, exclui um elemento pelo valor 

```python
cavaleiros.remove('Shun')
print(cavaleiros)
``` 
### Resultado
`['Athena', 'Seya', 'Aldebaran', 'Aldebaran', 'Shiryu', 'Yoga', 'Ikki', 'Shina', 'Maryn']`

## pop - exclui o ultimo elemtno da lista ou o indice informado 

```python
elemento = cavaleiros.pop()
cavaleiros.pop(0)
print(cavaleiros)
print(elemento)
``` 
### Resultado
```
['Seya', 'Aldebaran', 'Aldebaran', 'Shiryu', 'Yoga', 'Ikki', 'Shina']

Maryn
```

## indice - retorna o indice da primeira ocorrencia de um valor procurado 

```python
print(cavaleiros.index('Yoga'))

cavaleiros.pop(cavaleiros.index('Yoga'))
print(cavaleiros)
``` 
### Resultado
```
4

['Seya', 'Aldebaran', 'Aldebaran', 'Shiryu', 'Ikki', 'Shina']
```

## Alterando valor de um elemento da lista 

```python
cavaleiros[cavaleiros.index('Ikki')] = 'Ikki de fenix'
print(cavaleiros)
```
### Resultado
`['Seya', 'Aldebaran', 'Aldebaran', 'Shiryu', 'Ikki de fenix', 'Shina']`

## contabilizando quantidade de elementos repetidos 

```python
print(cavaleiros.count('Aldebaran'))
```
### Resultado
`2`

## sort ordena a lista de forma crescente 

Primeiro vamos criar uma lista numerica e outra de strings, contento algumas frutas, na sequencia ordenamos elas com o metodo sort()

```python

frutas = ['morango', 'maçã', 'abacaxi', 'kiwi',
          'amora', 'umbu', 'laranja', 'bergamota']

numeros = [9, 5, 81, 100, 33, 21, 2]

frutas.sort()
numeros.sort()

print(frutas)
print(numeros)
```
### Resultado
```
['abacaxi', 'amora', 'bergamota', 'kiwi', 'laranja', 'maçã', 'morango', 'umbu']

[2, 5, 9, 21, 33, 81, 100]
```

## inverte a ordem da lista

```python
frutas.reverse()
numeros.reverse()
print(frutas)
print(numeros)
```
### Resultado
```
['umbu', 'morango', 'maçã', 'laranja', 'kiwi', 'bergamota', 'amora', 'abacaxi']

[100, 81, 33, 21, 9, 5, 2]
```

## exclui um lista por completo ou um elemento especifico

```python
# exclui o primeiro elemento da lista, 
# podendo excluit qualquer um pelo indice
del frutas[0]

# exclui a lista inteira
del frutas
```

## Limpa a lista

 ```python
frutas.clear()
```


<div style="text-align: right">

[![voltar](../imagens/icons8-voltar-50.png)](./python.md)

</div>