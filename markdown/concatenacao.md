# O que é concatenação?  
Concatenação é o processo de unir duas ou mais strings (textos) em uma única string. No Python, isso pode ser feito de várias formas, dependendo do contexto e da necessidade do código.  

---
## Modos de concatenação

- [Operador +](#1-usando-o-operador-)
- [Join](#2-usando-join)
- [F-string](#3-usando-f-strings-python-36)
- [Format](#4-usando-format)
- [Usando %](#5-usando--formato-antigo-não-recomendado)
- [Concatenando listas](#6-usando--para-concatenar-em-loops)

---

## 1. Usando o operador `+`  
O operador `+` permite juntar duas ou mais strings.  

```python
nome = "João"
sobrenome = "Silva"
nome_completo = nome + " " + sobrenome
print(nome_completo)
```
**Saída:**  
```
João Silva
```
⚠️ **Atenção**: Se tentar concatenar strings com números diretamente, ocorrerá um erro!  

```python
idade = 25
print("Idade: " + idade)  # Isso gera um erro!
```
Para evitar o erro, converta o número para string usando `str()`:

```python
print("Idade: " + str(idade))
```
---

## 2. Usando `join()`  
O método `.join()` junta os elementos de uma lista de strings.  

```python
nomes = ["Maria", "Fernanda", "Oliveira"]
nome_completo = " ".join(nomes)
print(nome_completo)
```
**Saída:**  
```
Maria Fernanda Oliveira
```
---

## 3. Usando `f-strings` (Python 3.6+)  
F-strings permitem inserir variáveis dentro de strings de forma mais intuitiva.  

```python
nome = "Carlos"
idade = 30
mensagem = f"Meu nome é {nome} e eu tenho {idade} anos."
print(mensagem)
```
**Saída:**  
```
Meu nome é Carlos e eu tenho 30 anos.
```
---

## 4. Usando `.format()`  
O método `.format()` é outra maneira de formatar strings.  

```python
nome = "Ana"
cidade = "São Paulo"
mensagem = "Meu nome é {} e moro em {}.".format(nome, cidade)
print(mensagem)
```
**Saída:**  
```
Meu nome é Ana e moro em São Paulo.
```
Também pode ser usado com índices:  

```python
mensagem = "Meu nome é {0} e moro em {1}.".format(nome, cidade)
```
Ou nomeando os parâmetros:  

```python
mensagem = "Meu nome é {nome} e moro em {cidade}.".format(nome="Pedro", cidade="Curitiba")
```
---

## 5. Usando `%` (Formato Antigo, não recomendado)  
Antes do `.format()` e das `f-strings`, o Python usava `%` para formatar strings.  

```python
nome = "Beatriz"
idade = 27
mensagem = "Meu nome é %s e eu tenho %d anos." % (nome, idade)
print(mensagem)
```
**Saída:**  
```
Meu nome é Beatriz e eu tenho 27 anos.
```
⚠️ **Não é recomendado para novos projetos**, pois `.format()` e `f-strings` são mais legíveis e seguros.

---

## 6. Usando `+=` para concatenar em loops
Em alguns casos, pode ser necessário concatenar strings dentro de um loop.  

```python
frase = ""
for palavra in ["Eu", "adoro", "Python"]:
    frase += palavra + " "
print(frase.strip())  # strip() remove o espaço extra no final
```
**Saída:**  
```
Eu adoro Python
```

<div style="text-align: right">

[![voltar](../imagens/icons/icons8-voltar-50.png)](./python.md)

</div>