# Guia Básico de Python para Iniciantes

## Menu

- [Introdução](#introdução-à-linguagem-python)
- [Comentarios](#como-gerar-comentários)
- [Variaveis](#variáveis)
- [Entrada e saida de daos](#entrada-e-saída-de-dados)
- [Condicionais](#estruturas-condicionais)
- [Laços de repetição](#estruturas-de-repetição)
- [Listas](#listas)
- [Dicionarios](#dicionários)
- [Funções](#funções)

## 💡 Extra

- [Concatenação](./concatenacao.md)
- [Manipulação de Listas](./lista.md)
- [Manipulação de Dicionarios](./dicionario.md)

## Introdução à Linguagem Python

Python é uma linguagem de programação interpretada, de alto nível e com uma sintaxe simples e fácil de aprender. É amplamente utilizada em diversas áreas como desenvolvimento web, análise de dados, inteligência artificial e automação de tarefas.

Exemplo de código em Python:
```python
print("Olá, Mundo!")
```
**Saída:**
```
Olá, Mundo!
```

---
## Como Gerar Comentários
Comentários são usados para explicar o código e não são interpretados pelo Python.

- Comentário de uma linha: usa `#`
- Comentário de múltiplas linhas: usa três aspas `""" """` ou `''' '''`

**Exemplo:**
```python
# Este é um comentário de uma linha
print("Isso será exibido")

""" 
Este é um comentário
de múltiplas linhas
"""
print("Isso também será exibido")
```

**Saída:**
```
Isso será exibido
Isso também será exibido
```
---
## Variáveis
Variáveis são usadas para armazenar valores.

**Exemplo:**
```python
nome = "Maria"
idade = 25
altura = 1.65

print(nome, idade, altura)
```
**Saída:**
```
Maria 25 1.65
```
---

## Entrada e Saída de Dados
Podemos solicitar entrada do usuário com `input()` e exibir saída com `print()`.

**Exemplo:**
```python
nome = input("Digite seu nome: ")
print("Olá,", nome)
```
**Saída esperada:**
```
Digite seu nome: João
Olá, João
```

⚠️ [Veja mais detalhes sobre concatenação de strings](./concatenacao.md)

---

## Estruturas Condicionais
Usamos `if`, `elif` e `else` para tomar decisões.

**Exemplo:**
```python
idade = int(input("Digite sua idade: "))

if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```
**Saída esperada:**
```
Digite sua idade: 20
Você é maior de idade.
```

---
## Estruturas de Repetição
### `for`
Usado para percorrer sequências.

```python
for i in range(5):
    print(i)
```
**Saída:**
```
0
1
2
3
4
```

### `while`
Executa um bloco enquanto a condição for verdadeira.

```python
x = 0
while x < 5:
    print(x)
    x += 1
```
**Saída:**
```
0
1
2
3
4
```
---
## Listas
Listas armazenam múltiplos valores.

**Exemplo:**
```python
# indice     0        1       2
frutas = ["Maçã", "Banana", "Uva"]

print(frutas[0])  # Acessando o primeiro elemento
```
**Saída:**
```
Maçã
```

⚠️ [Veja mais detalhes para manipulação de listas](./lista.md)

---

## Dicionários
Dicionários armazenam pares chave-valor.

**Exemplo:**
```python
pessoa = {
    "nome": "Carlos", 
    "idade": 30
}

print(pessoa["nome"])
```
**Saída:**
```
Carlos
```
⚠️ [Veja mais detalhes para manipulação de dicionarios](./dicionario.md)

---

## Funções
Funções são blocos de código reutilizáveis.

**Exemplo:**
```python
def saudacao(nome):
    print("Olá,", nome)

saudacao("Ana")
```
**Saída:**
```
Olá, Ana
```

<div style="text-align: right">

[![voltar](../imagens/icons/icons8-voltar-50.png)](../README.md)

</div>