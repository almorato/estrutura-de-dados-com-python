# Módulo 3 — Pilhas (Stacks)

## O que é uma pilha?

Pilha é uma estrutura onde o último item que entra é o primeiro que sai. Em inglês: **LIFO** — Last In, First Out.

Analogia: uma pilha de pratos. Você coloca um prato em cima e pega de cima. Nunca do meio ou do fundo.

## Operações de uma pilha

| Operação | O que faz |
|---|---|
| `push` | Empilha um item (coloca no topo) |
| `pop` | Desempilha (retira do topo) |
| `peek` | Vê o topo sem remover |
| `is_empty` | Verifica se está vazia |

## Implementando com lista Python

Python não tem um tipo "pilha" nativo, mas uma lista já funciona perfeitamente:

```python
pilha = []

# push — adicionar no topo
pilha.append("primeiro")
pilha.append("segundo")
pilha.append("terceiro")
print(pilha)  # ["primeiro", "segundo", "terceiro"]

# pop — retirar do topo
item = pilha.pop()
print(item)   # "terceiro"
print(pilha)  # ["primeiro", "segundo"]

# peek — ver o topo sem remover
topo = pilha[-1]
print(topo)   # "segundo"

# verificar se está vazia
print(len(pilha) == 0)  # False
```

## Exemplo prático: verificar parênteses

Um uso real de pilha — verificar se os parênteses de uma expressão estão corretos:

```python
def parenteses_corretos(expressao):
    pilha = []
    for char in expressao:
        if char == "(":
            pilha.append(char)
        elif char == ")":
            if len(pilha) == 0:
                return False
            pilha.pop()
    return len(pilha) == 0

print(parenteses_corretos("(2 + 3) * (4 - 1)"))  # True
print(parenteses_corretos("(2 + 3))"))             # False
```

## Quando usar pilha

- Desfazer ações (Ctrl+Z) — a última ação feita é a primeira a ser desfeita
- Navegar no histórico do browser — voltar página por página
- Verificar estruturas aninhadas (parênteses, tags HTML)
- Chamadas de funções no computador (a pilha de execução)

## Exercício

Implemente uma pilha para simular o botão "desfazer" de um editor de texto simples:

1. Crie uma lista vazia chamada `historico`
2. Adicione 3 ações: "digitou 'Olá'", "digitou ' mundo'", "apagou 'mundo'"
3. Simule pressionar Ctrl+Z duas vezes (remova os dois últimos)
4. Imprima o estado final do histórico

Me mostre o código e o resultado.
