# Módulo 5 — Tuplas e Conjuntos (Sets)

## Tuplas

### O que é?

Tupla é como uma lista, mas **imutável** — depois de criada, não pode ser alterada.

```python
coordenadas = (10, 20)
rgb = (255, 128, 0)
pessoa = ("Alan", 35, "SP")
```

### Quando usar tupla em vez de lista?

Use tupla quando os dados não devem mudar:
- Coordenadas geográficas
- Cores RGB
- Chaves compostas em dicionários
- Retorno de múltiplos valores de uma função

```python
def min_max(numeros):
    return min(numeros), max(numeros)  # retorna uma tupla

menor, maior = min_max([3, 1, 4, 1, 5, 9])
print(menor, maior)  # 1 9
```

### Acesso e desempacotamento

```python
ponto = (3, 7)
print(ponto[0])  # 3
print(ponto[1])  # 7

x, y = ponto     # desempacotamento
print(x, y)      # 3 7
```

---

## Conjuntos (Sets)

### O que é?

Conjunto é uma coleção **sem ordem** e **sem itens repetidos**. Igual ao conceito matemático de conjunto.

```python
frutas = {"maçã", "banana", "laranja", "maçã"}
print(frutas)  # {"maçã", "banana", "laranja"} — removeu a repetição
```

### Operações principais

```python
a = {1, 2, 3, 4}
b = {3, 4, 5, 6}

print(a | b)   # união: {1, 2, 3, 4, 5, 6}
print(a & b)   # interseção: {3, 4}
print(a - b)   # diferença: {1, 2}

# adicionar e remover
a.add(10)
a.remove(1)

# verificar pertencimento (muito rápido)
print(3 in a)  # True
```

### Quando usar conjunto?

- Eliminar duplicatas de uma lista
- Verificar se um item existe (mais rápido que lista)
- Operações matemáticas entre grupos (união, interseção)

```python
# remover duplicatas de uma lista
lista_com_repeticao = [1, 2, 2, 3, 3, 3, 4]
sem_repeticao = list(set(lista_com_repeticao))
print(sem_repeticao)  # [1, 2, 3, 4]
```

## Exercício

1. Crie uma tupla com os dados de um produto: nome, preço e categoria
2. Crie duas listas de alunos de turmas diferentes (com alguns nomes repetidos)
3. Use conjuntos para descobrir: quais alunos estão nas duas turmas? Quais estão só na turma A?

Me mostre o código e o resultado.
