# Architecture Comparison

Este documento compara as duas arquiteturas implementadas neste projeto:

## 📌 Modelo Determinístico (Executor Fixo)

### Objetivo
Fornecer um fluxo de entrevista previsível, controlado e uniforme.

### Como funciona
- Perguntas definidas em sequência fixa
- Não há decisão adaptativa
- Cada resposta é validação de entrada para a próxima etapa

### Pontos Fortes
- Alta previsibilidade
- Fácil validação automatizada
- Fluxo padronizado para entrevistas repetíveis

### Limitações
- Não explora nuances do contexto
- Não aprofunda respostas automaticamente

---

## 📌 Modelo Adaptativo (Executor Dinâmico)

### Objetivo
Aproximar a experiência a uma entrevista conduzida por um entrevistador experiente.

### Como funciona
- Uma pergunta inicial fixa
- A IA decide o próximo passo com base na resposta
- Raciocínio contextual é aplicado

### Pontos Fortes
- Capacidade de aprofundar tópicos
- Exploração de lacunas ou ambiguidades
- Fluxo natural e menos rígido

### Limitações
- Menos previsível
- Difícil padronização
- Maior dependência de boa engenharia de prompt

---

## 🔎 Comparação Direta

| Critério                  | Executor Fixo       | Executor Dinâmico     |
|--------------------------|---------------------|------------------------|
| Previsibilidade          | Alta                | Média                  |
| Governança de Roteiro    | Alta                | Baixa                  |
| Adaptabilidade           | Baixa               | Alta                   |
| Complexidade de Prompt   | Média               | Alta                   |
| Experiência do Usuário   | Estruturada         | Conversacional         |
| Potencial de Profundidade| Limitado            | Elevado                |

---

## 🎯 Escolha de Arquitetura

Use o modelo fixo quando o objetivo for:
- Entrevistas padronizadas
- Sistemas com forte controle de discurso
- Verificação de requisitos objetivos

Use o modelo dinâmico quando o objetivo for:
- Aprofundar contexto
- Simular interlocução humana
- Gerar insights detalhados
