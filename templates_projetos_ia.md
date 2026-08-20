# Kit de Templates: Projetos de Inteligência Artificial

Este documento consolida os templates estruturados para criação, planejamento e apresentação de projetos de IA.

---

## 1. Template de Prompt Foco em IA (Framework de 14 Passos)

Copie e cole a estrutura abaixo no ChatGPT/Gemini/Claude para obter respostas de altíssima qualidade ao solicitar a criação de projetos, códigos ou planejamentos de IA. Preencha os campos em `[colchetes]`.

**1. Objetivo (Finalidade & Público-alvo)**
Desenvolver [descreva o que você quer, ex: um documento técnico / um script em Python] para um projeto de Inteligência Artificial focado em [Problema de Negócio]. O público-alvo é [quem vai ler/usar].

**2. Papel (Role/Tom/Autoridade)**
Atue como [ex: Cientista de Dados Sênior / Arquiteto de IA]. Use um tom [ex: profissional, técnico, didático].

**3. Contexto & Dados (Fontes/Não usar)**
- Dados: [Descreva a base de dados brevemente].
- O que usar: [ex: Técnicas modernas, boas práticas de MLOps].
- O que NÃO usar: [ex: Algoritmos defasados, jargões desnecessários].

**4. Tarefa (Instrução explícita)**
Sua tarefa é [descreva detalhadamente o que a IA deve fazer].
Aborde os seguintes pontos:
- [Ponto 1]
- [Ponto 2]

**5. Escopo & Restrições (Tempo/Segurança/Conformidade)**
- Tecnologias permitidas: [ex: Python, Scikit-learn, SQL].
- Conformidade: [ex: Respeitar a LGPD e remover PII].

**6. Definições operacionais**
- [Termo 1]: [Definição para alinhar o entendimento, ex: "MVP" = Produto Mínimo Viável focado em 1 única funcionalidade].

**7. Critérios de avaliação / Rubrica (Definition of Done)**
A resposta será avaliada com base em: [ex: Clareza técnica, viabilidade de implementação no contexto atual].

**8. Formato de saída (Contrato)**
A saída deve ser em formato Markdown, contendo seções claras e [ex: blocos de código documentados].

**9. Regras para ambiguidade e ausência de dados**
Se faltarem informações estruturais para o desenho final, [ex: faça até 3 perguntas antes de gerar a resposta / assuma premissas e liste-as no início do texto].

**10. Estilo de resposta**
Tom estruturado, direto, utilizando listas (bullet points) e negrito para destacar conceitos.

**11. Formato de resposta (skeleton canônico)**
Siga esta estrutura exata de tópicos:
[Cole aqui a estrutura de títulos (H1, H2, H3) desejada para a saída]

**12. Exemplos (few-shot curtos)**
[Forneça um exemplo de entrada e como deve ser a saída, se aplicável, ou apague este tópico].

**13. Checks finais (auto-verificação)**
Antes de gerar a resposta, valide silenciosamente se todos os requisitos, formatos e restrições foram estritamente cumpridos.

**14. Notas de design/observabilidade**
[Opcional, ex: Versão do prompt v1.0. Uso interno no time de dados].

---

## 2. Template de Plano de Projeto de IA

Utilize este esqueleto de documento para estruturar o planejamento técnico e de negócios de uma iniciativa de Machine Learning.

# Arquitetura e Planejamento: Projeto [Nome do Projeto]

## 1. Visão Geral do Problema e Objetivo
- **O Problema:** [Descrever o cenário atual e as dores de negócio]
- **Objetivo da IA:** [O que o modelo deve prever ou classificar]
- **Métrica de Sucesso (Negócio):** [ex: Aumento de 5% na retenção, redução de 10% em fraudes]

## 2. Coleta e Preparação de Dados
- **Fontes de Dados:** [Sistemas de origem, ex: CRM, ERP, Banco SQL, APIs]
- **Qualidade dos Dados:** Estratégias para lidar com valores nulos, registros duplicados e *outliers*.
- **Engenharia de Features:** [Novas variáveis que serão criadas a partir dos dados brutos para ajudar o modelo a aprender melhor]

## 3. Estratégia de Bases e Separação de Dados
- **Armazenamento:** [Onde os dados processados e raw ficarão armazenados]
- **Metodologia de Split:** [ex: 70% Treino, 15% Validação, 15% Teste; ou Time-Series Split se envolver fator tempo]
- **Prevenção de Vazamento (Data Leakage):** [Medidas para garantir que dados de teste/futuros não influenciem o treinamento (passado)]

## 4. Seleção de Algoritmos
- **Modelo Baseline:** [Modelo simples e altamente interpretável, ex: Regressão Logística ou Árvore de Decisão, usado para referência]
- **Modelos Avançados (Candidatos):** [ex: XGBoost, LightGBM, Random Forest, Redes Neurais]
- **Justificativa:** [Por que esses modelos se adequam especificamente aos dados e ao problema]

## 5. Estratégia de Treinamento e Otimização
- **Função de Custo (Loss Function):** [Métrica matemática interna do modelo a ser minimizada/maximizada]
- **Otimização de Hiperparâmetros:** [Técnica utilizada, ex: Grid Search, Random Search, Optuna]

## 6. Testes, Validação e Métricas
- **Métricas de Avaliação Técnica:** [ex: F1-Score, ROC-AUC, Precisão, Recall, RMSE]
- **Matriz de Confusão e Impacto:** [Custo e impacto dos Falsos Positivos vs Falsos Negativos para o negócio]
- **Testes de Viés (Bias) e Generalização:** [Garantia de que o modelo não está superajustado (overfitting) ou enviesado contra grupos específicos]

## 7. MLOps: Deploy e Monitoramento
- **Estratégia de Implantação:** [Como o modelo será consumido: API REST, processamento em lote (batch)]
- **Monitoramento Contínuo:** [Como será monitorado o Data Drift (mudanças na distribuição dos dados de entrada) e o Concept Drift (mudanças na relação entre os dados e a variável alvo)]

---

## 3. Template de Roteiro de Apresentação Executiva (Gamma.app / 3 Slides)

Utilize este roteiro para resumir projetos complexos de IA para a Diretoria, Stakeholders ou para alimentar o gerador de IA do Gamma.app.

# Slide 1: [Título Inspirador focado na Dor e Solução, ex: O Fim da Evasão de Clientes]
**Subtítulo:** [Resumo da oportunidade de negócio em uma única linha]
- **O Desafio Atual:** [O problema que custa tempo ou dinheiro hoje para a empresa]
- **A Limitação Atual:** [Por que as ferramentas atuais e regras de negócio manuais não funcionam mais]
- **A Visão com Inteligência Artificial:** [Como a IA muda o jogo resolvendo o problema de forma escalável e preditiva]

# Slide 2: [Título sobre os Bastidores da Solução, ex: Como a Nossa IA Funciona]
**Subtítulo:** [Uma visão simplificada e não-assustadora dos bastidores tecnológicos]
- **Nossos Dados:** [Aproveitamento de fontes seguras, históricas e ricas da própria empresa (Sistemas atuais)]
- **A Abordagem Inteligente:** [Em vez de premissas estáticas, o algoritmo aprende os padrões ocultos e se adapta ao comportamento real]
- **Integração Fluida:** [Como os resultados da IA se encaixam no fluxo de trabalho diário das equipes de forma invisível/sem atrito]

# Slide 3: [Título sobre Resultados e Próximos Passos, ex: O Impacto e a Jornada até a Entrega]
**Subtítulo:** [O que ganhamos, como validamos e quando entregamos o valor]
- **Impacto Esperado:** [Métrica principal focada em negócio, ex: Expectativa de redução de X% em perdas financeiras]
- **Validação Segura:** [Período de testes controlados (Shadow Mode / Teste A/B) antes da virada oficial em produção]
- **Próximos Passos (Roadmap):** [Ações imediatas e cronograma macro para a entrega do MVP]
