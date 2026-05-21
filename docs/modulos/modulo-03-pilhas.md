---
title: "Módulo 3 — Pilhas (Stacks)"
nav_order: 3
parent: Módulos
---

# Módulo 3 — Pilhas (Stacks)

## O que é?

LIFO — Last In, First Out. O último que entra é o primeiro que sai.

Analogia: pilha de pratos. Você coloca e retira sempre do topo.

## Operações

```python
pilha = []

pilha.append("A")   # push — empilha
pilha.append("B")
pilha.append("C")

pilha.pop()         # pop — desempilha ("C")
topo = pilha[-1]    # peek — vê o topo sem remover ("B")
```

## Quando usar

- Ctrl+Z (desfazer ações)
- Histórico de navegação (botão voltar)
- Verificar estruturas aninhadas (parênteses, tags)

---

[Fazer o quiz deste módulo](../quizzes/quiz-modulo-03){: .btn .btn-outline }
