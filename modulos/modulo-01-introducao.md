# Módulo 1 — Introdução às Estruturas de Dados

## O que é uma estrutura de dados?

Estrutura de dados é uma forma organizada de guardar e acessar informações no computador.

Pense assim: você pode guardar suas roupas jogadas no chão (funciona, mas é difícil achar algo) ou organizadas em gavetas por tipo (muito mais fácil). Estruturas de dados são essas "gavetas" para o seu programa.

## Por que isso importa?

Com a estrutura certa, seu programa:
- Encontra informações mais rápido
- Usa menos memória
- Fica mais fácil de entender e manter

## As estruturas que vamos aprender

| Estrutura | Analogia do dia a dia |
|---|---|
| Lista | Caderno de anotações — itens em ordem |
| Pilha | Pilha de pratos — o último que entra é o primeiro que sai |
| Fila | Fila do banco — o primeiro que chega é o primeiro atendido |
| Tupla | Endereço de uma casa — não muda |
| Conjunto | Lista de convidados únicos — sem repetição |
| Dicionário | Agenda telefônica — nome → número |
| Árvore | Organograma de empresa — hierarquia |

## Dois conceitos importantes

**Complexidade de tempo** — quanto tempo uma operação leva conforme os dados crescem. Não precisa decorar fórmulas agora — vamos sentir isso na prática.

**Mutável vs imutável** — alguns tipos podem ser alterados depois de criados (mutáveis), outros não (imutáveis). Listas são mutáveis. Tuplas são imutáveis.

## Exercício

No Python, execute estas linhas e observe o que acontece:

```python
# Uma lista simples
frutas = ["maçã", "banana", "laranja"]
print(frutas)
print(frutas[0])   # primeiro item
print(len(frutas)) # quantos itens tem
```

Depois me diga: o que apareceu na tela e o que cada linha fez?
