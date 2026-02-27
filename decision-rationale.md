# Decision Rationale

Este documento explica a lógica de design por trás das duas arquiteturas.

## 🎯 Por que dois modelos?

Conduzir entrevistas por IA pode ter diferentes objetivos:
1. **Fluxo padronizado** — ideal para contratações em larga escala
2. **Fluxo adaptativo** — ideal para análises profundas e consultoria técnica

Separar esses dois modelos permite:
- Comparar resultados
- Analisar trade-offs
- Aprender engenharia de prompt

## 📌 Design do Executor Fixo

Principais razões:
- Controle de estado
- Sequência precisa de tópicos
- Evitar perguntas redundantes
- Geração de saída apenas após conclusão

Decisões de engenharia:
- Sequência linear
- Confirmação explícita antes de gerar resumo
- Regras rígidas para evitar respostas fora de escopo

---

## 📌 Design do Executor Dinâmico

Principais razões:
- Simular um entrevistador humano
- Capacidade de adaptar perguntas
- Aprofundar em respostas que sejam vagas ou incompletas

Decisões de engenharia:
- Análise semântica da resposta anterior
- Geração de perguntas de follow-up
- Raciocínio condicional para guiar fluxo

---

## 🧠 Critérios de Avaliação

A decisão de qual modelo utilizar pode ser guiada pelos seguintes critérios:

### 1. Objetivo do usuário
- Definição de requisitos técnicos
- Entrevista exploratória

### 2. Nível de detalhamento desejado
- Perfil de vaga
- Avaliação detalhada de competências

### 3. Necessidade de repeatability
- Padronização para pipelines de contratação

---

## ✅ Conclusão

Ter duas abordagens co-existindo permite:
- Estudo comparativo
- Evolução do sistema
- Escolha flexible conforme necessidade
