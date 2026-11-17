# Plano de evolução documental e técnica

Este documento separa o que já está disponível no repositório, o que precisa de evidência adicional e o que é proposta de evolução. A prioridade evita apresentar um blueprint como se fosse uma implantação concluída.

## P0 — fundação verificável

- Código-fonte reproduzível da aplicação.
- Dependências, ambiente e comandos de execução.
- Testes automatizados e contratos de API.
- Dicionário de dados e modelo relacional.
- Pipeline de dados executável.
- Dados de demonstração versionados.

## P1 — maturidade de engenharia

- Backtesting e comparação de previsões.
- Model Card e versionamento de modelos.
- ADRs para decisões arquiteturais.
- C4, fluxo de dados e linhagem.
- Qualidade de dados com regras e resultados.
- GitHub Actions para testes, links e documentação.
- Observabilidade, SLOs e runbooks.
- Simulador financeiro reproduzível.

## P2 — apresentação e operação

- Portal MkDocs Material.
- Storybook ou catálogo equivalente do Design System.
- Diagramas DBML, D2 e Draw.io editáveis.
- Gráficos interativos e relatórios HTML.
- Roteiros de demonstração e capturas reais.
- RACI, backlog técnico, FinOps e plano de piloto.

## Critério de aceite

Uma entrega só deve ser marcada como concluída quando houver uma evidência verificável: código, teste, contrato, resultado calculado, captura real ou documento de decisão. Quando a evidência não existir, registre o item como **proposto** ou **pendente**.

## Próxima sequência recomendada

1. Tornar a execução local reproduzível.
2. Conectar README, documentação e código.
3. Validar dados, métricas e simulações.
4. Publicar o portal e automatizar a auditoria documental.
