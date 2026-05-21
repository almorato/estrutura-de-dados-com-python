# Módulo 4 — Filas (Queues)

## O que é uma fila?

Fila é uma estrutura onde o primeiro item que entra é o primeiro que sai. Em inglês: **FIFO** — First In, First Out.

Analogia: fila do banco. Quem chegou primeiro é atendido primeiro. Ninguém fura a fila.

## Diferença entre fila e pilha

| | Pilha | Fila |
|---|---|---|
| Entra por | cima | atrás |
| Sai por | cima (LIFO) | frente (FIFO) |
| Analogia | pilha de pratos | fila do banco |

## Implementando com deque

Python tem um tipo otimizado para filas chamado `deque` (double-ended queue), do módulo `collections`:

```python
from collections import deque

fila = deque()

# enqueue — entrar na fila
fila.append("cliente 1")
fila.append("cliente 2")
fila.append("cliente 3")
print(fila)  # deque(["cliente 1", "cliente 2", "cliente 3"])

# dequeue — sair da fila (primeiro que entrou)
atendido = fila.popleft()
print(atendido)  # "cliente 1"
print(fila)      # deque(["cliente 2", "cliente 3"])

# ver quem está na frente
print(fila[0])   # "cliente 2"

# verificar se está vazia
print(len(fila) == 0)  # False
```

## Por que não usar lista simples?

Tecnicamente funciona, mas `list.pop(0)` é lento em listas grandes — ele precisa mover todos os outros itens. O `deque.popleft()` é muito mais eficiente.

## Exemplo prático: fila de impressão

```python
from collections import deque

fila_impressao = deque()

# documentos chegando
fila_impressao.append("relatorio.pdf")
fila_impressao.append("planilha.xlsx")
fila_impressao.append("apresentacao.pptx")

# impressora processa um por vez
while fila_impressao:
    documento = fila_impressao.popleft()
    print(f"Imprimindo: {documento}")
```

## Quando usar fila

- Fila de impressão
- Processamento de tarefas em ordem de chegada
- Sistema de mensagens (chat, notificações)
- BFS — busca em largura em grafos

## Exercício

Simule um sistema de atendimento:

1. Crie uma fila com 4 clientes: "João", "Maria", "Pedro", "Ana"
2. Atenda (remova) os dois primeiros
3. Chegue mais um cliente: "Carlos"
4. Imprima quem ainda está na fila e quem é o próximo a ser atendido

Me mostre o código e o resultado.
