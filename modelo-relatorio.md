# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS: PHARMAEFFICIENCY

**Data:** 22 de Janeiro de 2026  
**Empresa:** Abstergo Industries  
**Responsável:** Claudean Soares

## 1. Introdução
Este relatório detalha a estratégia de otimização de infraestrutura da **Abstergo Industries**, focada na redução de custos operacionais através da migração para um modelo de processamento em nuvem. O objetivo central foi a substituição de sistemas de alto custo fixo por uma arquitetura **Serverless** (sem servidor), garantindo que a empresa pague apenas pelo processamento efetivamente utilizado durante a operação farmacêutica.

## 2. Descrição do Projeto (Pilar de Processamento)

O projeto foi estruturado em três frentes tecnológicas complementares para garantir a máxima eficiência financeira:

**Etapa 1: Processamento sob Demanda**
- **Ferramenta:** AWS Lambda
- **Foco:** Execução Reativa (Pilar de Custo Variável)
- **Caso de Uso:** Implementado para processar os cálculos de descontos e convênios no checkout. A lógica de negócio é acionada apenas quando um item é bipado, eliminando a necessidade de manter servidores ligados 24/7. A viabilidade financeira deste modelo foi validada através de simulações técnicas.

**Etapa 2: Orquestração de Fluxos de Trabalho**
- **Ferramenta:** AWS Step Functions
- **Foco:** Automação de Workflows Complexos
- **Caso de Uso:** Utilizado para coordenar a jornada de venda de medicamentos controlados. O serviço gerencia a sequência de validações entre a farmácia e o SNGPC (órgãos reguladores), garantindo integridade de dados sem custos de infraestrutura ociosa.



**Etapa 3: Arquitetura Orientada a Eventos**
- **Ferramenta:** Amazon EventBridge
- **Foco:** Desacoplamento e Mensageria
- **Caso de Uso:** Atua como o barramento central que notifica o setor de compras sempre que o estoque atinge um nível crítico. Essa abordagem evita que sistemas de monitoramento fiquem consultando o banco de dados constantemente, economizando recursos de IOPS e tráfego.



## 3. Conclusão
A implementação da arquitetura proposta resulta em uma infraestrutura resiliente e financeiramente inteligente. Com base nos testes realizados, estima-se uma redução de custos de processamento superior a 70% em comparação ao modelo tradicional. Esta transição posiciona a **Abstergo Industries** como uma operação tecnologicamente avançada e sustentável.

A busca pela eficiência técnica é também um compromisso com a integridade. Como afirma a tradição católica através de **São Bento**: 
> "Ora et Labora" (Ora e Trabalha). 

O trabalho realizado com ordem e dedicação é o caminho para o progresso e para a excelência profissional.

## 4. Anexos Técnicos
- **Simulação de Viabilidade Econômica:** [Acesse o Notebook Técnico (.ipynb)](./notebooks/simulador_custos_aws.ipynb)
- **Definição de Infraestrutura:** Arquivo de configuração JSON para Step Functions.
