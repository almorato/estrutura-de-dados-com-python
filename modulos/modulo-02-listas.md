# Módulo 2 — Listas e Operações Fundamentais

## O que é uma lista em Python?

Uma lista é uma coleção ordenada de itens que pode ser alterada. É a estrutura de dados mais usada em Python.

```python
numeros = [1, 2, 3, 4, 5]
nomes = ["Ana", "Bruno", "Carla"]
misturado = [1, "texto", True, 3.14]  # pode misturar tipos
```

## Operações essenciais

### Adicionar itens
```python
frutas = ["maçã", "banana"]

frutas.append("laranja")      # adiciona no final
frutas.insert(0, "uva")       # adiciona na posição 0 (início)

print(frutas)  # ["uva", "maçã", "banana", "laranja"]
```

### Remover itens
```python
frutas.remove("banana")   # remove pelo valor
frutas.pop()              # remove o último
frutas.pop(0)             # remove pelo índice
```

### Acessar itens
```python
print(frutas[0])    # primeiro item
print(frutas[-1])   # último item
print(frutas[1:3])  # fatia: do índice 1 até o 2
```

### Percorrer a lista
```python
for fruta in frutas:
    print(fruta)
```

### Outras operações úteis
```python
len(frutas)           # quantidade de itens
"maçã" in frutas      # verifica se existe
frutas.sort()         # ordena
frutas.reverse()      # inverte
frutas.index("uva")   # retorna o índice do item
```

## Quando usar listas

Use lista quando:
- A ordem dos itens importa
- Você precisa adicionar ou remover itens
- Pode ter itens repetidos

## Exercício

Crie uma lista com 5 nomes de colegas. Depois:
1. Adicione mais um nome no final
2. Remova o segundo nome
3. Imprima a lista em ordem alfabética

Me mostre o código e o resultado.
