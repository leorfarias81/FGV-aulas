# Kit de Templates: Projetos de Inteligência Artificial

Este documento consolida os templates estruturados para criação de prompts, planejamento técnico e apresentação de projetos de IA.

---

## 1. Template 1: Criação de Prompts (Genérico)

Copie esta estrutura em branco e preencha os campos para criar qualquer tipo de prompt avançado, seguindo estritamente os 14 passos estruturais.

**1. Objetivo (Finalidade & Público-alvo)**
- O que entregar e para quem (ex.: gestor, leigo, equipe técnica).
- `[Preencha aqui]`

**2. Papel (Role/Tom/Autoridade)**
- Persona, tom desejado e limites de atuação.
- `[Preencha aqui]`

**3. Contexto & Dados (Fontes/Não usar)**
- Que dados/links usar; o que não usar; premissas e limites.
- `[Preencha aqui]`

**4. Tarefa (Instrução explícita)**
- Passos/entregáveis concretos (ex.: "avaliar", "comparar", "sintetizar").
- `[Preencha aqui]`

**5. Escopo & Restrições (Tempo/Segurança/Conformidade)**
- Prazos, ferramentas permitidas, privacidade, referências obrigatórias.
- `[Preencha aqui]`

**6. Definições operacionais**
- Conceitos que regem a avaliação/produção (ex.: "clareza", "objetividade").
- `[Preencha aqui]`

**7. Critérios de avaliação / Rubrica (Definition of Done)**
- Critérios mensuráveis e limiares de aceitação (ex.: alta/moderada/baixa; 0-2 por critério).
- `[Preencha aqui]`

**8. Formato de saída (Contrato)**
- Preferir JSON Schema / function calling; alternativa: Markdown com seções obrigatórias.
- Campos required, limites de tamanho, política para ausências (null).
- `[Preencha aqui]`

**9. Regras para ambiguidade e ausência de dados**
- Quando devolver "Insuficiente"; quando perguntar antes de responder; mensagens de erro padrão.
- `[Preencha aqui]`

**10. Estilo de resposta**
- Tom profissional, conciso, estruturado; evitar juízos subjetivos.
- `[Preencha aqui]`

**11. Formato de resposta (skeleton canônico)**
- Cole aqui o modelo exato de saída (JSON/Markdown) a ser seguido.
- `[Preencha aqui]`

**12. Exemplos (few-shot curtos)**
- 1-2 exemplos de entrada -> saída aderentes ao contrato.
- `[Preencha aqui]`

**13. Checks finais (auto-verificação)**
- Validar JSON/sections; checar rubrica; citar fontes/IDs quando aplicável.
- `[Preencha aqui]`

**14. Notas de design/observabilidade (opcional)**
- Versão do prompt, parâmetros, seed, logging para auditoria e reuso.
- `[Preencha aqui]`

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

---

## 4. Template para Criação Interativa de Notebook de Projeto

Utilize este prompt direto para instruir o ChatGPT (ou outra IA) a analisar a estrutura dos projetos já existentes no repositório da FGV e criar um novo Jupyter Notebook alinhado a esse padrão. A instrução força a IA a trabalhar de forma iterativa, validando decisões com você antes de escrever o código.

```text
Utilize os exemplos de projetos (https://github.com/mfidosjr/FGV-aulas/tree/main/aplicacoes-de-negocio) para criar um notebook de um projeto de IA (anexa o seu pdf) .... – trabalhe de modo iterativo, e me pergunte sobre todas as decisões antes de criar o projeto.
```
