# Auditoria de visualizações interativas

## Escopo

A aplicação usa gráficos analíticos em dashboards, previsão, estoque, impacto financeiro, qualidade e monitoramento. Diagramas arquiteturais e fluxogramas permanecem estáticos porque sua finalidade é explicar estrutura, não explorar séries de dados.

## Matriz de auditoria

| Visualização | Localização | Fonte | Interações | Status |
|---|---|---|---|---|
| Risco por centro de distribuição | Painel semanal (S01) | Fixture/API de alertas | Tabela acessível, barras comparáveis, navegação por teclado | Corrigido |
| Tendência de demanda e estoque | Painel semanal (S01) | Série demonstrativa de 14 dias | Hover, foco por teclado, tooltip, legenda liga/desliga, zoom e restaurar | Corrigido |
| Estoque e validade por lote | Estoque (S07) | Lotes do cenário | Tabela de dados e filtros da tela | Verificar evolução |
| Previsão de demanda | Previsões (S08) | Série temporal demonstrativa | Linha, tabela alternativa e filtros | Verificar evolução |
| Rede de CDs e logística | Transferências (S09) | CDs, prazo e restrições | Seleção de origem/destino e simulação | Verificar evolução |
| Impacto financeiro | Financeiro (S10) | Cenário de simulação | Comparação de alternativas e valores | Verificar evolução |
| Qualidade dos dados | Dados (S11) | Indicadores de qualidade | Cards, definições e tabela alternativa | Verificar evolução |
| Modelos e erro | Modelos (S12) | Métricas documentadas | Tabela de versões e métricas | Verificar evolução |
| Relatórios | Relatórios (S13) | Resumo do período | Tabelas e filtros | Verificar evolução |

## Interações do gráfico de tendência

O gráfico do S01 oferece:

- tooltip no mouse;
- foco e leitura pelo teclado;
- data, demanda prevista e estoque disponível no tooltip;
- legenda para mostrar ou ocultar séries;
- zoom e restauração;
- texto alternativo e instrução equivalente sem depender do hover;
- comportamento responsivo.

A implementação usa SVG sem dependência adicional de biblioteca. Essa escolha mantém o bundle pequeno e permite controlar acessibilidade, estados e integração com o estado da aplicação. Plotly permanece uma alternativa para séries analíticas futuras que exijam zoom contínuo, exportação ou grandes volumes.

## Testes e evidências

A verificação deve confirmar:

1. renderização sem erro JavaScript;
2. foco nos pontos com Tab;
3. tooltip com data e unidades;
4. legenda alterando a visibilidade da série;
5. zoom e restauração;
6. leitura alternativa por texto/tabela;
7. adaptação em 390 px, 768 px e 1440 px.

O gráfico arquitetural, Mermaid e imagens de apoio não entram no critério de interatividade analítica.
