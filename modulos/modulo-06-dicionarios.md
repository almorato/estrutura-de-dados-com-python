# Módulo 6 — Dicionários e Tabelas Hash

## O que é um dicionário?

Dicionário é uma estrutura que guarda pares **chave → valor**. Como uma agenda: você busca pelo nome e encontra o telefone.

```python
agenda = {
    "Ana": "99999-1111",
    "Bruno": "99999-2222",
    "Carla": "99999-3333"
}

print(agenda["Ana"])  # "99999-1111"
```

## Operações principais

```python
# criar
produto = {"nome": "Notebook", "preco": 3500, "estoque": 10}

# acessar
print(produto["nome"])          # "Notebook"
print(produto.get("cor", "N/A"))  # "N/A" — sem erro se não existir

# adicionar ou atualizar
produto["cor"] = "prata"
produto["preco"] = 3200

# remover
del produto["estoque"]
produto.pop("cor")

# verificar se chave existe
print("nome" in produto)  # True

# percorrer
for chave, valor in produto.items():
    print(f"{chave}: {valor}")
```

## O que é uma Tabela Hash?

Tabela Hash é o mecanismo por dentro do dicionário. Quando você faz `dict["chave"]`, Python não percorre tudo — ele calcula um "endereço" da chave instantaneamente. Por isso dicionários são extremamente rápidos.

Você não precisa implementar isso manualmente — o dicionário Python já faz isso por você.

## Casos de uso comuns

### Contar ocorrências
```python
texto = "banana"
contagem = {}

for letra in texto:
    contagem[letra] = contagem.get(letra, 0) + 1

print(contagem)  # {"b": 1, "a": 3, "n": 2}
```

### Agrupar dados
```python
alunos = [
    {"nome": "Ana", "turma": "A"},
    {"nome": "Bruno", "turma": "B"},
    {"nome": "Carla", "turma": "A"},
]

por_turma = {}
for aluno in alunos:
    turma = aluno["turma"]
    if turma not in por_turma:
        por_turma[turma] = []
    por_turma[turma].append(aluno["nome"])

print(por_turma)  # {"A": ["Ana", "Carla"], "B": ["Bruno"]}
```

## Quando usar dicionário

- Buscar por identificador (ID, nome, código)
- Contar frequência de itens
- Agrupar dados por categoria
- Armazenar configurações e propriedades de objetos

## Exercício

Crie um dicionário que represente um aluno com: nome, idade, notas (lista com 3 notas) e curso. Depois:
1. Calcule e exiba a média das notas
2. Adicione um campo "aprovado" com True se a média for >= 6
3. Imprima todos os dados do aluno

Me mostre o código e o resultado.
