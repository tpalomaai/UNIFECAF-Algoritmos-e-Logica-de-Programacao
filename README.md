# 📦 Sistema de Gestão de Peças, Qualidade e Armazenamento

Projeto desenvolvido na disciplina de **Algoritmos e Lógica de Programação** — UniFECAF, 2026.

Autora: **Paloma Ai Tsuchinaga**

---

## 📋 Sobre o Projeto

Este programa simula um sistema de controle de qualidade industrial feito em Python.

Ele funciona como uma esteira de fábrica: cada peça que chega é inspecionada, aprovada ou reprovada, organizada em caixas e, no final, gera um relatório completo com tudo que aconteceu.

---

## ⚙️ O que o programa faz

1. Recebe os dados de cada peça (peso, cor e comprimento)
2. Verifica se a peça está dentro dos padrões
3. Aprova ou reprova a peça com o motivo
4. Coloca as peças aprovadas em caixas de 10 unidades
5. Fecha a caixa automaticamente quando chega em 10 peças
6. Gera um relatório final ao encerrar

---

## ✅ Critérios de Aprovação

| Critério      | Valor aceito         |
|---------------|----------------------|
| Peso          | Entre 95g e 105g     |
| Cor           | Azul ou Verde        |
| Comprimento   | Entre 10cm e 20cm    |

> Uma peça pode ser reprovada por um, dois ou todos os critérios ao mesmo tempo.

---

## 📊 Relatório Final

Ao encerrar, o programa exibe:

- Total de peças processadas
- Total de peças aprovadas
- Total de peças reprovadas
- Total de caixas fechadas
- Peças que ficaram na caixa incompleta (se houver)
- IDs de todas as peças reprovadas (se houver)

---

## 🧠 Conceitos utilizados

- **Condições** (`if`, `and`, `or`) — para tomar decisões sobre cada peça
- **Repetição** (`while True` + `break`) — para processar várias peças em sequência
- **Funções** — `verificar_peca()` e `gerar_relatorio()` para organizar o código
- **Listas** — para guardar peças na caixa, caixas fechadas e IDs reprovados

---

## 📁 Estrutura do Projeto

```
📦 controle-de-producao
 ┣ 🎬 Paloma_Ai_Tsuchinga_-_Sistema_de_Gestão_de_Peças_Qualidade_e_Armazenamento.mp4
 ┣ 📄 Trabalho_-_Gestão_de_Peças_Qualidade_e_Armazenamento.pdf
 ┣ 🖼️ Código_-_Sistema_de_Gestão_de_Peças_Qualidade_e_Armazenamento.png
 ┣ 💻 visual-code-sistema-de-gestao-de-pecas-qualidade-e-armazenamento.py
 ┣ 📄 README.md
```
