---
title: "Módulo 4 — Filas (Queues)"
nav_order: 4
parent: Módulos
---

# Módulo 4 — Filas (Queues)

## O que é?

FIFO — First In, First Out. O primeiro que entra é o primeiro que sai.

Analogia: fila do banco. Quem chegou primeiro é atendido primeiro.

## Operações

```python
from collections import deque

fila = deque()

fila.append("cliente 1")    # enqueue — entra na fila
fila.append("cliente 2")
fila.append("cliente 3")

fila.popleft()              # dequeue — sai da fila ("cliente 1")
print(fila[0])              # ver o próximo sem remover
```

## Por que deque e não lista?

`deque.popleft()` é muito mais eficiente que `list.pop(0)` em listas grandes.

## Quando usar

- Fila de impressão
- Processamento de tarefas em ordem de chegada
- Sistema de mensagens e notificações

---

[Fazer o quiz deste módulo](../quizzes/quiz-modulo-04){: .btn .btn-outline }
