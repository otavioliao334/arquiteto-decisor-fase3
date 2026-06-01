# ADR 0001 – Estratégia de Nuvem e Escalabilidade

## Status
Aceito

## Contexto
O crescimento do sistema exige maior flexibilidade de infraestrutura e capacidade de adaptação a picos de acesso.

## Decisão
Adotar uma estratégia de **PaaS em Cloud**, priorizando **escalabilidade horizontal**.

## Alternativas Consideradas
- IaaS: maior controle, porém maior custo operacional.
- Serverless: limitações de controle e complexidade de depuração.

## Consequências
- Facilidade de escalabilidade
- Redução de custos operacionais
- Dependência do provedor de nuvem

## Fundamentação Teórica
Segundo Fowler (2015), arquiteturas modernas se beneficiam da escalabilidade horizontal para sistemas distribuídos.
