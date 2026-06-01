# ADR 0002 – Padrões de Resiliência

## Status
Aceito

## Contexto
Falhas em sistemas distribuídos são inevitáveis e precisam ser tratadas de forma controlada.

## Decisão
Implementar **API Gateway** e **Circuit Breaker**.

## Alternativas Consideradas
- Comunicação direta entre serviços
- Retry ilimitado

## Consequências
- Isolamento de falhas
- Redução de efeito cascata
- Complexidade adicional

## Fundamentação Teórica
Segundo Nygard (2018), o Circuit Breaker é essencial para resiliência em microsserviços.
