---
title: "Módulo 6 — Dicionários e Tabelas Hash"
nav_order: 6
parent: Módulos
---

# Módulo 6 — Dicionários e Tabelas Hash

## O que é?

Pares chave → valor. Como uma agenda telefônica: você busca pelo nome e encontra o número.

## Operações principais

```python
produto = {"nome": "Notebook", "preco": 3500}

produto["cor"] = "prata"                    # adicionar
produto["preco"] = 3200                     # atualizar
del produto["cor"]                          # remover
print(produto.get("cor", "N/A"))            # sem erro se não existir

for chave, valor in produto.items():        # percorrer
    print(f"{chave}: {valor}")
```

## Tabela Hash

O mecanismo interno do dicionário que permite acesso por chave em tempo constante — sem percorrer todos os itens.

## Quando usar

- Buscar por identificador (nome, ID, código)
- Contar frequência de itens
- Agrupar dados por categoria

---

[Fazer o quiz deste módulo](../quizzes/quiz-modulo-06){: .btn .btn-outline }
