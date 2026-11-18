# Decisões arquiteturais

| Decisão adotada | Motivo | Implicação |
| --- | --- | --- |
| Gerar a base com semente fixa | Reproduzir indicadores, erros de qualidade e cenários na demonstração | Um piloto precisa versionar e proteger seus próprios dados |
| Calcular riscos e cenários no navegador | Disponibilizar a experiência sem infraestrutura de dados em execução | Filtros são mantidos em memória e o simulador principal encerra na análise |
| Priorizar o lote que vence primeiro | Aproximar o consumo projetado da operação e explicar as sobras | O cálculo depende de validade, disponibilidade e demanda confiáveis |
| Usar fórmula determinística para a demanda | Facilitar a conferência do cálculo e demonstrar o fluxo | A faixa de ±17% é ilustrativa. A precisão exigiria avaliação temporal com dados autorizados |
| Validar transferência antes de estimar benefício | Impedir que um resultado financeiro positivo substitua critérios operacionais | A decisão final exige análise humana e confirmação de custos, prazo e validade |

[Arquitetura publicada](arquitetura.md) · [Evidências](evidencias.md) · [Evolução proposta](maturity-roadmap.md)
