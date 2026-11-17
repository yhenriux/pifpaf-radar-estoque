# Guia editorial e voz documental

## Princípio

**Clareza para compreender. Evidências para confiar. Instruções para reproduzir.**

A documentação do Radar combina rigor de engenharia, clareza didática e visão estratégica. O texto deve servir a três leitores:

- **Diretoria:** valor projetado, riscos e decisões apoiadas.
- **Coordenação e arquitetura:** viabilidade, governança, dependências e trade-offs.
- **Engenharia:** implementação, testes, contratos e reprodução.

## Regras de escrita

1. Escreva em português brasileiro, com voz ativa e frases objetivas.
2. Defina siglas na primeira ocorrência e mantenha a terminologia estável.
3. Comece pela pergunta que a página responde.
4. Explique o conceito, aplique-o ao Radar, mostre um exemplo e indique como verificar.
5. Apresente números com unidade, período, origem, método e limitação.
6. Conecte indicadores a efeitos operacionais e econômicos.
7. Diferencie explicitamente **implementado**, **testado**, **especificado**, **proposto** e **simulado**.
8. Não invente métricas, integrações, tecnologias ou resultados.
9. Prefira verbos operacionais: executar, validar, comparar, registrar e monitorar.
10. Evite jargões desnecessários, superlativos e linguagem promocional.

## Estrutura padrão de uma página

1. Objetivo
2. Contexto
3. Fundamentos
4. Funcionamento ou arquitetura
5. Exemplo aplicado
6. Implementação, fórmula ou contrato
7. Verificação
8. Limitações e decisões
9. Próximos passos

Páginas de API, ADRs e runbooks podem usar modelos específicos, mas devem preservar a distinção entre evidência e proposta.

## Evidência e rastreabilidade

Toda afirmação importante deve apontar para código, teste, contrato, configuração, métrica ou registro de decisão. Para cada indicador, documente definição, fórmula, unidade, período, fonte e forma de reprodução.

A jornada editorial deve permitir sair de uma conclusão executiva, chegar ao indicador que a sustenta e, em seguida, alcançar o método de cálculo e a evidência técnica.

## Vocabulário do produto

| Termo técnico | Forma preferida para leitores gerais |
|---|---|
| snapshot | base de dados de referência |
| lead time | prazo de transporte |
| baseline | previsão de referência |
| FEFO | prioridade para o lote que vence primeiro |
| SKU | código do produto |
| ERP | sistema corporativo |
| WAPE | erro ponderado da previsão |

Use o termo técnico quando ele for necessário para uma implementação ou contrato. Na primeira ocorrência, escreva o termo por extenso e explique seu papel no Radar.
