# Dicionario

É um conjunto de chaves e valores que distinguem um objeto. Estas chaves nos chamamos de KEYS e seus valores de VALUES. É um tipo especial de variavel python identificada pelas {}.  

## Criando um dicionario

```python
pessoa = {
    'nome': 'Luciano',
    'idade': 30 ,
    'cidade': 'São Paulo'
}

print(pessoa)
```

## Verifincando as chaves do dicionario
```python
    print(pessoa.keys())
```

### Resultado:
`dict_keys(['nome', 'idade', 'cidade'])`

## Verificando os valores do dicionario
```python
print(pessoa.values())
```

### Resultado:
`dict_values(['Luciano', 30, 'São Paulo'])`

## Olhando valores especificos de um dicionario

```python
pessoa['nome']
```
### resultado:
`'Luciano'`

## Atribuindo um novo valor a uma chave
```python
pessoa['cidade'] = 'Brasilia'
```

### Resultado

valor anterior
`{'nome': 'Luciano', 'idade': 30, 'cidade': 'São Paulo'}`

valor apos alteração
`{'nome': 'Luciano', 'idade': 30, 'cidade': 'Brasilia'}`


## excluindo uma chave e seu valor
```python
del pessoa['idade']

pessoa.pop('cidade')

print(pessoa)
```

### Resultado
`{'nome': 'Luciano', 'email': 'luciano@teste.com'}`

## Percorrendo uma lista de dicionarios

Primeiro iremos declarar uma lista com varios dicionarios

```python
alunos = [
    {'nome': 'Daniel', 'cidade':'Aguas claras'},
    {'nome': 'Marcos', 'cidade':'recanto'},
    {'nome': 'Luana', 'cidade':'brasilia'},
    {'nome': 'Francineide', 'cidade':'Ceilandia'}
]
```

### Percorrendo lista e printando cada dicionario
```python
for indice, aluno in enumerate(alunos):
    print(indice , aluno)
```
#### Resultado
```
0 {'nome': 'Daniel', 'cidade': 'Aguas claras'}
1 {'nome': 'Marcos', 'cidade': 'recanto'}
2 {'nome': 'Luana', 'cidade': 'brasilia'}
3 {'nome': 'Francineide', 'cidade': 'Ceilandia'}
```

### Printando um aluno especifico da lista usando o indice
```python
print(alunos[2])
```
#### Resultado
`{'nome': 'Luana', 'cidade': 'brasilia'}`

### Printando um valor especifico em um dicionario

```python
print(alunos[2]['cidade'])
```
#### Resultado

`brasilia`



<div style="text-align: right">

[![voltar](../imagens/icons8-voltar-50.png)](./python.md)

</div>