# Quiz — Módulo 4: Filas (Queues)

## Instruções
Para fazer o quiz interativamente, diga ao Claude:
> "Quero fazer o quiz do módulo 4"

---

## Perguntas

### 1. O que significa FIFO?
a) First In, Fixed Order
b) Fast Input, Fast Output
c) First In, First Out
d) Full Index, First Out

### 2. Por que usar `deque` em vez de lista simples para implementar filas?
a) Porque lista não suporta strings
b) Porque `deque.popleft()` é mais eficiente que `list.pop(0)`
c) Porque `deque` suporta mais tipos de dados
d) Não há diferença prática

### 3. De qual módulo Python o `deque` é importado?
a) `queue`
b) `structures`
c) `collections`
d) `deque`

### 4. Em uma fila com os itens ["A", "B", "C", "D"], após dois `popleft()` e um `append("E")`, qual é o estado da fila?
a) ["A", "B", "E"]
b) ["C", "D", "E"]
c) ["E", "C", "D"]
d) ["B", "C", "D", "E"]

### 5. Qual cenário é mais adequado para usar uma fila?
a) Histórico de navegação no browser
b) Verificar parênteses em expressões matemáticas
c) Processar pedidos de um restaurante em ordem de chegada
d) Armazenar coordenadas geográficas

---

## Gabarito (para o instrutor)
1. c
2. b
3. c
4. b
5. c

## Critérios de avaliação
- 5 acertos: Excelente — pode avançar com confiança
- 3-4 acertos: Bom — revise os pontos errados antes de avançar
- 0-2 acertos: Revise o módulo antes de continuar
