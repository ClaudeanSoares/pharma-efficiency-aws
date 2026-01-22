# 💊 PharmaEfficiency: Redução de Custos e Otimização com AWS Serverless

## 🎯 Visão do Projeto
Ao analisar a infraestrutura da **Abstergo Industries**, identifiquei que o modelo de servidores tradicionais gerava custos fixos elevados, independentemente da demanda real da operação farmacêutica. Minha proposta com este projeto foi redesenhar o sistema para uma arquitetura **Serverless**, garantindo que a tecnologia trabalhe de forma enxuta e eficiente.

## 🛠️ O que implementei para reduzir custos:

Minha estratégia focou em transformar despesas fixas em variáveis, utilizando o poder da nuvem AWS:

### 1. Processamento sob Demanda com AWS Lambda
Substituí instâncias ligadas 24/7 por funções **Lambda** para processar cálculos de convênios e descontos.
* **Impacto:** Eliminamos o pagamento por ociosidade. Agora, a empresa só é tarifada durante o milissegundo de execução de cada venda.

### 2. Fluxos Inteligentes com AWS Step Functions
Utilizei o **Step Functions** para gerenciar a aprovação de receitas de medicamentos controlados.
* **Impacto:** Reduzi a complexidade do código e a necessidade de manter servidores ativos esperando por validações externas. O fluxo agora é orquestrado de forma nativa e econômica.

### 3. Monitoramento Reativo (Amazon EventBridge)
Implementei um barramento de eventos para gatilhos de reposição de estoque.
* **Impacto:** Acabei com o "polling" constante no banco de dados. O sistema só reage quando um evento real acontece, economizando processamento e tráfego de dados.

---

## 📂 Organização do Repositório
* **[Relatório Estratégico](./modelo-relat%C3%B3rio.md)**: Minha análise técnica completa e defesa da solução.
* **[Simulador de Custos (Python)](./cadernos/simulador_custos_aws.ipynb)**: Notebook onde validei matematicamente a economia gerada.
* **[Infraestrutura JSON](./step-function-definition.json)**: Arquivo de configuração da máquina de estados na raiz do projeto.

---

## 💭 Reflexão
Como ensina a sabedoria de **São Josémaria Escrivá**: 
> "Acaba as coisas. — Põe nelas a última pedra."

Este README é a última pedra deste projeto. Busquei a perfeição na organização para que o resultado técnico reflita o cuidado e a ordem que dediquei a cada etapa.

---
**Projeto desenvolvido durante a curso Santander 2025 - Ciência de Dados com Python.**
