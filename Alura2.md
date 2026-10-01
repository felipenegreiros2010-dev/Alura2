# 🎟️ Projeto: Controle de Ingressos do Evento Escolar

> Programa que verifica se alunos, monitores e convidados cabem nos **100 ingressos** disponíveis e se o limite de **20 convidados** foi respeitado.

---

## 📑 Sumário

1. [Sobre o projeto](#-sobre-o-projeto)
2. [Regras de negócio](#-regras-de-negócio)
3. [Prompt](#-prompt)
4. [Casos de teste](#-casos-de-teste)
5. [Como usar](#-como-usar)
6. [Checklist de entrega](#-checklist-de-entrega)

---

## 📌 Sobre o projeto

Uma escola vai realizar um evento com **100 ingressos** disponíveis para alunos, monitores e convidados. Para tudo ocorrer bem, o total de pessoas não pode ultrapassar a quantidade de ingressos. Além disso, a direção impôs uma regra: no máximo **20 convidados** no total, mesmo que sobrem ingressos.

O objetivo é criar um programa que leia as quantidades, faça as verificações e exiba uma mensagem adequada para cada situação.

> 💡 **Dica:** realize este desafio em seu próprio projeto (repositório) para deixar sua entrega mais significativa.

---

## 📏 Regras de negócio

| # | Regra | Valor |
|---|---|---|
| 1 | Total de ingressos disponíveis | **100** |
| 2 | Limite máximo de convidados | **20** |
| 3 | Total de pessoas | `alunos + monitores + convidados` |
| 4 | Condição de ingressos | total de pessoas **≤ 100** |
| 5 | Condição de convidados | convidados **≤ 20** |

---

## 🤖 Prompt

Copie o prompt abaixo e cole na IA de sua preferência. Se quiser outra linguagem, troque apenas o trecho `Python`.

````text
Atue como um professor de programação paciente e objetivo. Quero que você crie um programa em Python para o seguinte problema.

CONTEXTO
Estou ajudando a organizar um evento na minha escola, que tem 100 ingressos disponíveis para alunos, monitores e convidados. O total de pessoas não pode ultrapassar a quantidade de ingressos. Além disso, a direção da escola impôs uma regra: é permitido haver, no máximo, 20 convidados no total, mesmo que sobrem ingressos.

O QUE O PROGRAMA DEVE FAZER
1. Ler do usuário a quantidade de alunos, de monitores e de convidados.
2. Calcular o total de pessoas (alunos + monitores + convidados).
3. Verificar se o total de pessoas cabe nos 100 ingressos disponíveis.
4. Verificar se o número de convidados está dentro do limite de 20.
5. Exibir uma mensagem adequada para cada uma das 4 situações possíveis:
   - Total dentro dos 100 ingressos e convidados dentro do limite de 20.
   - Total dentro dos 100 ingressos, mas convidados acima de 20.
   - Total acima de 100 ingressos, mas convidados dentro do limite de 20.
   - Total acima de 100 ingressos e convidados acima de 20.

REQUISITOS TÉCNICOS
- Use constantes nomeadas para os limites (TOTAL_INGRESSOS = 100 e LIMITE_CONVIDADOS = 20), sem "números mágicos" no meio do código.
- Valide a entrada: aceite apenas números inteiros maiores ou iguais a zero. Se o usuário digitar algo inválido, mostre um aviso e peça novamente.
- Separe o código em funções (por exemplo: ler número, verificar regras, exibir mensagem).
- Mostre na saída o total de pessoas e quantos ingressos sobram ou faltam.
- Use nomes de variáveis claros, em português, e comentários curtos explicando as partes principais.
- Use apenas a biblioteca padrão do Python.

FORMATO DA RESPOSTA
1. O código completo em um único bloco.
2. Uma explicação curta, em linguagem simples, de como o programa funciona.
3. Uma tabela com pelo menos 5 casos de teste (entrada e saída esperada), incluindo os valores limite (exatamente 100 pessoas e exatamente 20 convidados).
4. Sugestões de como eu poderia melhorar o projeto depois (por exemplo: salvar em arquivo, criar interface, repetir o cálculo para vários eventos).

IMPORTANTE
Explique o código de um jeito que um estudante iniciante consiga entender e reproduzir. Não use dados pessoais em nenhum exemplo.
````

---

## 🧪 Casos de teste

Use estes casos para conferir se o programa gerado está correto (inclui os valores limite):

| Alunos | Monitores | Convidados | Total | Ingressos | Convidados | Resultado esperado |
|---:|---:|---:|---:|:---:|:---:|---|
| 60 | 10 | 10 | 80 | ✅ ok | ✅ ok | Tudo certo, evento pode ocorrer (sobram 20 ingressos) |
| 70 | 10 | 20 | 100 | ✅ ok (limite) | ✅ ok (limite) | Tudo certo, ingressos esgotados |
| 50 | 10 | 25 | 85 | ✅ ok | ❌ acima de 20 | Ingressos suficientes, mas excede o limite de convidados |
| 80 | 15 | 10 | 105 | ❌ acima de 100 | ✅ ok | Convidados ok, mas faltam 5 ingressos |
| 80 | 15 | 30 | 125 | ❌ acima de 100 | ❌ acima de 20 | Excede os ingressos e o limite de convidados |
| 0 | 0 | 0 | 0 | ✅ ok | ✅ ok | Tudo certo (nenhuma pessoa inscrita) |

---

## ▶️ Como usar

1. Cole o prompt na IA e gere o código.
2. Salve o código em um arquivo, por exemplo `ingressos.py`.
3. Execute no terminal:

```bash
python ingressos.py
```

4. Teste com os casos da tabela acima e confira as mensagens.
5. **Revise o código gerado**: leia, entenda e ajuste o que for necessário. A IA pode errar e não deve ser a única fonte.

---

## ✅ Checklist de entrega

- [ ] Criei o projeto em um repositório próprio
- [ ] Usei o prompt e gerei o código
- [ ] Li e entendi o código antes de entregar
- [ ] O programa lê alunos, monitores e convidados
- [ ] Verifica o limite de 100 ingressos
- [ ] Verifica o limite de 20 convidados
- [ ] Exibe uma mensagem adequada para cada situação
- [ ] Testei todos os casos da tabela, inclusive os valores limite
- [ ] Incluí este README no repositório

---

<sub>Projeto do desafio "Controle de ingressos do evento escolar". Bons estudos! 🚀</sub>
