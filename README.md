# Mini Projeto – Arquiteto Decisor (Fase 3)

## Visão Executiva do Sistema

Este projeto representa a evolução arquitetural de um sistema originalmente monolítico para um **ambiente baseado em Cloud e Microsserviços**. O objetivo é aumentar **escalabilidade, resiliência e manutenibilidade**, atendendo às demandas de crescimento e disponibilidade do sistema.

O sistema resolve o problema de processamento e gerenciamento de dados de usuários e operações de negócio, permitindo que diferentes domínios funcionais evoluam de forma independente.

Atualmente, na **Fase 4**, o sistema encontra-se arquitetado em microsserviços, com comunicação controlada, padrões de resiliência aplicados e infraestrutura preparada para escalabilidade horizontal.

---

## Arquitetura – Diagrama C4 (Containers)

```mermaid
flowchart LR
    User[Usuário]
    APIGW[API Gateway]
    
    User --> APIGW
    
    APIGW --> Auth[Serviço de Autenticação]
    APIGW --> Core[Serviço Principal]
    APIGW --> Notify[Serviço de Notificações]

    Core --> DB[(Banco de Dados)]
    Auth --> DB
