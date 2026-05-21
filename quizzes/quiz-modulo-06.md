# Quiz — Módulo 6: Dicionários e Tabelas Hash

## Instruções
Para fazer o quiz interativamente, diga ao Claude:
> "Quero fazer o quiz do módulo 6"

---

## Perguntas

### 1. Como acessar o valor de uma chave em um dicionário sem gerar erro se a chave não existir?
a) `dict["chave"]`
b) `dict.get("chave", valor_padrão)`
c) `dict.find("chave")`
d) `dict.search("chave")`

### 2. O que é uma Tabela Hash no contexto de dicionários Python?
a) Um tipo especial de lista ordenada
b) Um mecanismo interno que permite acesso rápido por chave sem percorrer tudo
c) Uma estrutura que ordena as chaves automaticamente
d) Um banco de dados embutido no Python

### 3. Dado `d = {"a": 1, "b": 2}`, o que acontece ao executar `d["c"] = 3`?
a) Erro — a chave "c" não existe
b) A chave "c" é adicionada com valor 3
c) O dicionário é reiniciado
d) O valor 3 substitui o valor da chave "a"

### 4. Qual estrutura é mais adequada para contar quantas vezes cada palavra aparece em um texto?
a) Lista
b) Pilha
c) Dicionário
d) Conjunto

### 5. Como percorrer tanto as chaves quanto os valores de um dicionário ao mesmo tempo?
a) `for item in dict:`
b) `for chave, valor in dict.items():`
c) `for chave in dict.keys(), valor in dict.values():`
d) `dict.foreach()`

---

## Gabarito (para o instrutor)
1. b
2. b
3. b
4. c
5. b

## Critérios de avaliação
- 5 acertos: Excelente — pode avançar com confiança
- 3-4 acertos: Bom — revise os pontos errados antes de avançar
- 0-2 acertos: Revise o módulo antes de continuar
