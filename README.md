# 📦 Sistema de Gestão de Peças, Qualidade e Armazenamento

Projeto desenvolvido na disciplina de **Algoritmos e Lógica de Programação** — UniFECAF, 2026.

Autora: **Paloma Ai Tsuchinaga**

---

## 🎬 Video Pitch

🔗 [Assistir no YouTube](https://www.youtube.com/watch?v=wUajZKP0PHs)

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

## 🧪 Exemplos de Entrada

| Peça | Peso | Cor | Comprimento | Resultado |
|------|------|-----|-------------|-----------|
| 1 | 100g | azul | 15cm | ✅ Aprovada (1/10) |
| 2 | 80g | verde | 12cm | ❌ Reprovada — peso errado |
| 3 | 98g | verde | 10cm | ✅ Aprovada (2/10) |
| 4 | 102g | amarelo | 18cm | ❌ Reprovada — cor errada |
| 5 | 95g | azul | 20cm | ✅ Aprovada (3/10) |
| 6 | 103g | verde | 13cm | ✅ Aprovada (4/10) |
| 7 | 101g | verde | 25cm | ❌ Reprovada — comprimento errado |
| 8 | 99g | azul | 14cm | ✅ Aprovada (5/10) |
| 9 | 105g | verde | 19cm | ✅ Aprovada (6/10) |
| 10 | 60g | azul | 30cm | ❌ Reprovada — peso e comprimento errado |
| 11 | 97g | azul | 11cm | ✅ Aprovada (7/10) |
| 12 | 104g | verde | 16cm | ✅ Aprovada (8/10) |
| 13 | 96g | azul | 18cm | ✅ Aprovada (9/10) |
| 14 | 100g | verde | 12cm | ✅ Aprovada (10/10) — 📦 caixa fechada! |

<details>
<summary>Ver entradas detalhadas</summary>

**Peça 1 — Aprovada (1/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `100` / Cor: `azul` / Comprimento: `15`

**Peça 2 — Reprovada (peso errado)**
- Há uma nova peça na esteira? `sim`
- Peso: `80` / Cor: `verde` / Comprimento: `12`

**Peça 3 — Aprovada (2/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `98` / Cor: `verde` / Comprimento: `10`

**Peça 4 — Reprovada (cor errada)**
- Há uma nova peça na esteira? `sim`
- Peso: `102` / Cor: `amarelo` / Comprimento: `18`

**Peça 5 — Aprovada (3/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `95` / Cor: `azul` / Comprimento: `20`

**Peça 6 — Aprovada (4/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `103` / Cor: `verde` / Comprimento: `13`

**Peça 7 — Reprovada (comprimento errado)**
- Há uma nova peça na esteira? `sim`
- Peso: `101` / Cor: `verde` / Comprimento: `25`

**Peça 8 — Aprovada (5/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `99` / Cor: `azul` / Comprimento: `14`

**Peça 9 — Aprovada (6/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `105` / Cor: `verde` / Comprimento: `19`

**Peça 10 — Reprovada (dois motivos: peso e comprimento)**
- Há uma nova peça na esteira? `sim`
- Peso: `60` / Cor: `azul` / Comprimento: `30`

**Peça 11 — Aprovada (7/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `97` / Cor: `azul` / Comprimento: `11`

**Peça 12 — Aprovada (8/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `104` / Cor: `verde` / Comprimento: `16`

**Peça 13 — Aprovada (9/10)**
- Há uma nova peça na esteira? `sim`
- Peso: `96` / Cor: `azul` / Comprimento: `18`

**Peça 14 — Aprovada (10/10 — caixa fechada!)**
- Há uma nova peça na esteira? `sim`
- Peso: `100` / Cor: `verde` / Comprimento: `12`

**Encerrar**
- Há uma nova peça na esteira? `nao`

</details>

### Resultado esperado no relatório

```
Total de peças processadas : 14
Total de peças aprovadas   : 10
Total de peças reprovadas  : 4
Total de caixas fechadas   : 1
```

---

## 📁 Estrutura do Projeto

```
📦 controle-de-producao
 ┣ 🎬 Paloma_Ai_Tsuchinga_-_Sistema_de_Gestão_de_Peças_Qualidade_e_Armazenamento.mp4
 ┣ 📄 Trabalho_-_Gestão_de_Peças_Qualidade_e_Armazenamento.pdf
 ┣ 🖼️ Código_-_Sistema_de_Gestão_de_Peças_Qualidade_e_Armazenamento.png
 ┣ 💻 visual-code-sistema-de-gestao-de-pecas-qualidade-e-armazenamento.py
 ┣ 📄 README.md
