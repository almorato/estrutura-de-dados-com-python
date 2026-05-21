# Módulo 8 — Projeto Final: Escolhendo a Estrutura Certa

## O que você aprendeu

| Estrutura | Característica principal | Use quando |
|---|---|---|
| Lista | Ordenada, mutável | Sequências que mudam |
| Pilha | LIFO — último a entrar, primeiro a sair | Desfazer ações, histórico |
| Fila | FIFO — primeiro a entrar, primeiro a sair | Processar em ordem de chegada |
| Tupla | Imutável | Dados que não devem mudar |
| Conjunto | Sem repetição, sem ordem | Eliminar duplicatas, comparar grupos |
| Dicionário | Chave → valor | Buscar por identificador |
| Árvore | Hierárquica | Busca rápida, dados hierárquicos |

## Como escolher a estrutura certa

Faça estas perguntas:

1. **Os dados têm ordem?** → Lista ou Tupla
2. **Os dados mudam?** → se não, Tupla; se sim, Lista
3. **Precisa de duplicatas?** → se não, Conjunto
4. **Precisa buscar por chave?** → Dicionário
5. **Processa em ordem de chegada?** → Fila
6. **Precisa desfazer?** → Pilha
7. **Dados hierárquicos ou busca rápida em volume?** → Árvore

## Projeto Final

Escolha **um** dos cenários abaixo e implemente a solução completa em Python:

---

### Cenário A — Sistema de Biblioteca

Implemente um sistema simples com:
- Cadastro de livros (título, autor, disponível: sim/não)
- Busca por título
- Fila de espera para livros indisponíveis
- Histórico de empréstimos (últimos 5)

---

### Cenário B — Analisador de Texto

Dado um texto qualquer:
- Conte a frequência de cada palavra
- Liste as 5 palavras mais usadas
- Mostre quantas palavras únicas existem
- Verifique se duas palavras específicas aparecem no texto

---

### Cenário C — Agenda de Contatos

Implemente uma agenda com:
- Adicionar contato (nome, telefone, email)
- Buscar por nome
- Listar contatos em ordem alfabética
- Remover contato
- Histórico das últimas 3 buscas realizadas

---

## Como entregar

Me mostre o código completo e explique:
1. Quais estruturas você usou em cada parte
2. Por que escolheu cada uma
3. O que você mudaria se o sistema precisasse crescer muito (milhões de registros)

Parabéns por chegar até aqui!
