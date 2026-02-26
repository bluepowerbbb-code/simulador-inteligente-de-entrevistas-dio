

---

📘 AI Interview Simulator

Simulador de entrevistas técnicas estruturadas utilizando engenharia de prompt para controle de fluxo conversacional.

Este projeto apresenta duas arquiteturas distintas de condução de entrevista com IA, permitindo comparar:

🔹 Modelo Determinístico (Fluxo Fixo)

🔹 Modelo Adaptativo (Fluxo Dinâmico)


A proposta é demonstrar evolução arquitetural em relação ao modelo tradicional apresentado em aula na Digital Innovation One.


---

🎯 Objetivo do Projeto

Demonstrar como diferentes estratégias de engenharia de prompt impactam:

Controle de estado

Governança da resposta

Adaptabilidade

Complexidade conversacional

Previsibilidade do sistema



---

🧠 Arquiteturas Implementadas

🔹 V1 — Modelo Determinístico (Fluxo Fixo)

Características

Ordem de perguntas predefinida

Uma pergunta por vez

Proibição explícita de pular etapas

Geração de resumo apenas após confirmação do usuário

Estrutura rígida de 4 blocos:

1. Título da vaga


2. Senioridade


3. Stack técnica


4. Soft skills




Vantagens

Alta previsibilidade

Controle total do fluxo

Redução de alucinação estrutural

Fácil auditoria


Indicado para

Sistemas críticos

Aplicações corporativas

Ambientes que exigem padronização



---

🔹 V2 — Modelo Adaptativo (Fluxo Dinâmico)

Características

Primeira pergunta fixa

Próximas perguntas definidas dinamicamente pela IA

Análise contextual da resposta anterior

Capacidade de aprofundamento técnico

Fluxo não linear


Funcionamento

A IA:

1. Analisa semanticamente a resposta do usuário


2. Identifica lacunas ou pontos de aprofundamento


3. Decide qual pergunta é mais relevante em seguida


4. Constrói uma entrevista personalizada



Vantagens

Maior naturalidade

Maior profundidade técnica

Simula entrevistador humano real

Capacidade adaptativa


Indicado para

Produtos SaaS

Simuladores avançados

Avaliação técnica personalizada



---

🔬 Comparação Arquitetural

Critério	Modelo Fixo	Modelo Dinâmico

Controle de Fluxo	Alto	Moderado
Adaptabilidade	Baixa	Alta
Complexidade	Baixa	Alta
Previsibilidade	Alta	Média
Sofisticação de Prompt	Média	Alta
Simulação Realista	Média	Alta



---

🏗 Estrutura do Repositório

/prompts/
   executor-fixed.md
   executor-dynamic.md

/docs/
   architecture-comparison.md
   decision-rationale.md

/examples/
   structured-example.md
   adaptive-example.md


---

⚙ Engenharia de Prompt

Este projeto demonstra:

Controle sequencial de geração

Bloqueio condicional de saída

Separação entre fase de coleta e fase de análise

Simulação de estado conversacional

Tomada de decisão baseada em contexto (V2)



---

🚀 Evolução em Relação ao Modelo Base

Enquanto o modelo tradicional executa um fluxo simples de perguntas, este projeto:

Implementa controle explícito de governança

Introduz arquitetura adaptativa

Separa executor fixo de executor dinâmico

Permite comparação entre paradigmas

Demonstra design de sistemas baseados em prompt



---

🧩 Próximas Evoluções

Sistema de scoring automático

Avaliação por critérios ponderados

Geração de relatório estruturado em JSON

Integração com API

Interface Web



---

🏁 Conclusão

Este repositório não é apenas um simulador de entrevistas.

É um estudo comparativo de arquiteturas conversacionais baseadas em IA, explorando controle determinístico versus inteligência adaptativa.


---

