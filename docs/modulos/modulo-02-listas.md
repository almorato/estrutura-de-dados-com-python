---
title: "Módulo 2 — Listas e Operações Fundamentais"
nav_order: 2
parent: Módulos
---

# Módulo 2 — Listas e Operações Fundamentais

## O que é uma lista?

Coleção ordenada e mutável de itens. É a estrutura mais usada em Python.

## Operações principais

```python
frutas = ["maçã", "banana", "laranja"]

frutas.append("uva")       # adiciona no final
frutas.insert(0, "kiwi")   # adiciona na posição 0
frutas.remove("banana")    # remove pelo valor
frutas.pop()               # remove o último
frutas.sort()              # ordena

print(frutas[0])           # primeiro item
print(frutas[-1])          # último item
print(len(frutas))         # quantidade de itens
print("maçã" in frutas)    # verifica se existe
```

## Quando usar

- A ordem dos itens importa
- Você precisa adicionar ou remover itens
- Pode ter itens repetidos

---

[Fazer o quiz deste módulo](../quizzes/quiz-modulo-02){: .btn .btn-outline }
