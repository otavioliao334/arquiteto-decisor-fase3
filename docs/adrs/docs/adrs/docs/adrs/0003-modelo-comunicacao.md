# ADR 0003 – Modelo de Comunicação

## Status
Aceito

## Contexto
A comunicação entre microsserviços impacta diretamente desempenho e acoplamento.

## Decisão
Adotar **comunicação síncrona via HTTP/REST** para os fluxos principais.

## Alternativas Consideradas
- Comunicação assíncrona com mensageria
- Eventos distribuídos

## Consequências
- Simplicidade de implementação
- Maior acoplamento temporal
- Facilidade de depuração

## Fundamentação Teórica
De acordo com Richardson (2019), REST é adequado para cenários com necessidade de resposta imediata.
