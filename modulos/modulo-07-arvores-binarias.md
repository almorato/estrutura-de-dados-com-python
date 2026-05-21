# Módulo 7 — Árvores Binárias

## O que é uma árvore?

Árvore é uma estrutura hierárquica — como um organograma de empresa ou a árvore genealógica de uma família.

```
        10          ← raiz (root)
       /  \
      5    15       ← nós filhos
     / \     \
    3   7     20    ← folhas (sem filhos)
```

## Vocabulário básico

| Termo | Significado |
|---|---|
| Raiz (root) | O nó do topo, sem pai |
| Nó (node) | Cada elemento da árvore |
| Filho (child) | Nó abaixo de outro |
| Pai (parent) | Nó acima de outro |
| Folha (leaf) | Nó sem filhos |
| Altura | Quantidade de níveis |

## Árvore Binária de Busca (BST)

Na **Árvore Binária de Busca**:
- Valores menores ficam à **esquerda**
- Valores maiores ficam à **direita**

Isso permite encontrar qualquer valor rapidamente — sem precisar checar tudo.

## Implementando em Python

```python
class No:
    def __init__(self, valor):
        self.valor = valor
        self.esquerda = None
        self.direita = None

class ArvoreBinaria:
    def __init__(self):
        self.raiz = None

    def inserir(self, valor):
        if self.raiz is None:
            self.raiz = No(valor)
        else:
            self._inserir(self.raiz, valor)

    def _inserir(self, no, valor):
        if valor < no.valor:
            if no.esquerda is None:
                no.esquerda = No(valor)
            else:
                self._inserir(no.esquerda, valor)
        else:
            if no.direita is None:
                no.direita = No(valor)
            else:
                self._inserir(no.direita, valor)

    def em_ordem(self, no):
        if no:
            self.em_ordem(no.esquerda)
            print(no.valor, end=" ")
            self.em_ordem(no.direita)

# usando a árvore
arvore = ArvoreBinaria()
for numero in [10, 5, 15, 3, 7, 20]:
    arvore.inserir(numero)

arvore.em_ordem(arvore.raiz)  # 3 5 7 10 15 20 — em ordem crescente!
```

## Por que árvores são úteis?

- Busca muito mais rápida que listas em grandes volumes de dados
- Organização hierárquica natural (pastas, menus, categorias)
- Base para estruturas mais avançadas (banco de dados, sistemas de arquivos)

## Quando usar

- Dados que precisam ser buscados frequentemente e em grande volume
- Representar hierarquias (categorias, estruturas organizacionais)
- Implementar autocompletar e dicionários de palavras

## Exercício

Use o código acima e:
1. Insira os valores: 8, 4, 12, 2, 6, 10, 14
2. Imprima em ordem (em_ordem) — o resultado deve ser crescente
3. Diga: se eu quiser encontrar o valor 6, por quais nós a árvore passaria antes de achar?

Me mostre o código e a resposta à pergunta 3.
