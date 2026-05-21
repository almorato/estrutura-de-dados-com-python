---
title: "Módulo 5 — Tuplas e Conjuntos (Sets)"
nav_order: 5
parent: Módulos
---

# Módulo 5 — Tuplas e Conjuntos (Sets)

## Tuplas

Imutáveis — não podem ser alteradas após criadas.

```python
coordenadas = (-23.5, -46.6)   # latitude, longitude
pessoa = ("Alan", 35, "SP")

x, y = coordenadas              # desempacotamento
```

**Quando usar:** dados fixos como coordenadas, retorno de múltiplos valores.

---

## Conjuntos (Sets)

Sem ordem e sem repetição.

```python
a = {1, 2, 3, 4}
b = {3, 4, 5, 6}

a | b   # união: {1, 2, 3, 4, 5, 6}
a & b   # interseção: {3, 4}
a - b   # diferença: {1, 2}

# remover duplicatas de uma lista
sem_repeticao = list(set([1, 2, 2, 3, 3, 3]))
```

**Quando usar:** eliminar duplicatas, verificar pertencimento, operações entre grupos.

---

[Fazer o quiz deste módulo](../quizzes/quiz-modulo-05){: .btn .btn-outline }
