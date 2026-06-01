# Software Architecture Document (SAD) – Fase 3

## 1. Introdução
Este documento descreve a arquitetura de software adotada na Fase 4 do Mini Projeto Arquiteto Decisor. O objetivo é apresentar as decisões arquiteturais tomadas para a evolução do sistema em um contexto de Cloud Computing e Microsserviços, garantindo escalabilidade, resiliência e manutenibilidade.

## 2. Objetivo do Sistema
O sistema tem como objetivo fornecer uma solução digital escalável para processamento e gerenciamento de operações de negócio, permitindo o atendimento eficiente de múltiplos usuários simultaneamente.

## 3. Visão Geral da Arquitetura
A arquitetura adotada é baseada em microsserviços independentes, hospedados em ambiente de nuvem, com comunicação centralizada por meio de um API Gateway. Cada microsserviço é responsável por um domínio específico do negócio, permitindo evolução independente e melhor isolamento de falhas.

## 4. Estilo Arquitetural
- Arquitetura de Microsserviços  
- Arquitetura Distribuída  
- Cloud Computing (PaaS)  

## 5. Componentes da Arquitetura
- **API Gateway:** ponto único de entrada para os clientes  
- **Serviço de Autenticação:** responsável por controle de acesso e segurança  
- **Serviço Principal de Negócio:** executa as regras centrais do sistema  
- **Serviço de Notificações:** responsável por envio de mensagens e alertas  
- **Banco de Dados:** armazenamento persistente das informações  

## 6. Requisitos Não Funcionais
- Escalabilidade horizontal  
- Alta disponibilidade  
- Resiliência a falhas  
- Segurança  
- Manutenibilidade  

## 7. Infraestrutura
O sistema é executado em ambiente de nuvem utilizando serviços gerenciados (PaaS), permitindo provisionamento automático de recursos e suporte à escalabilidade conforme a demanda.

## 8. Decisões Arquiteturais
As principais decisões arquiteturais estão documentadas por meio de ADRs localizados na pasta `/docs/adrs`, abordando:
- Estratégia de nuvem e escalabilidade  
- Padrões de resiliência  
- Modelo de comunicação entre serviços  

## 9. Riscos e Mitigações
- **Falhas em serviços:** mitigadas com padrões de resiliência  
- **Sobrecarga de requisições:** mitigada com escalabilidade horizontal  
- **Dependência de provedor:** mitigada por boas práticas de arquitetura  

## 10. Considerações Finais
A arquitetura proposta atende aos requisitos atuais do sistema e fornece uma base sólida para futuras evoluções, garantindo flexibilidade, robustez e alinhamento com boas práticas modernas de engenharia de software.
