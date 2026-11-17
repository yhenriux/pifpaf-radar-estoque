# Guia de documentação

## Comece pelo valor

O Radar apoia decisões semanais de estoque, validade e abastecimento. Combina leitura dos lotes, previsão de demanda, simulação de alternativas e registro de decisões para comparar **perda potencial, ruptura e custo logístico**. A solução aqui descrita é **um case demonstrativo independente** para uma operação de alimentos congelados.

[Aplicação pública](https://radar-estoque-validade-pifpaf.yhenri-ux.chatgpt.site/) · [Voltar ao README](../README.md)

### Para cada público

| Público | Primeiro documento | Pergunta respondida |
|---|---|---|
| Diretoria | [Demo executiva](demo.md) | Qual problema resolvemos e qual valor se projeta? |
| Gestão de operação | [Jornada do usuário](produto/jornada.md) | Que ação avaliar, aprovar e acompanhar? |
| Engenharia de dados | [Dados](dados.md) | Quais fontes, transformações e testes sustentam decisões? |
| Engenharia de IA | [Modelos](modelos.md) | Como medir erro, incerteza e confiança? |
| Arquitetura e segurança | [Arquitetura](arquitetura.md) e [Governança](governanca.md) | Quais componentes, controles e trade-offs? |
| Avaliação externa | [Reproduzir](reproducao.md) e [Evidências](evidencias.md) | Quais partes existem, quais precisam de código e como comprovar? |

### Estrutura de informação

A documentação combina quatro tipos de conteúdo, conforme os princípios de organização do [Diátaxis](https://diataxis.fr/): **tutorial**, **guia de tarefa**, **referência** e **explicação**. Cada página distingue **fato observado**, **especificação do blueprint** e **proposta futura**.

### Métricas e transparência

Não confunda **ganho projetado**, **valor em risco**, **custo evitável** e **resultado realizado**. Os cenários usam dados sintéticos e devem ser reproduzidos por rotinas versionadas quando o código for publicado. A experiência de produto pode priorizar mensagens executivas, enquanto a documentação preserva integralmente as premissas de simulação.

### Inventário documental

- [Arquitetura](arquitetura.md), [Dados](dados.md), [Modelos](modelos.md)
- [Jornadas e telas](produto/jornada.md)
- [Governança](governanca.md), [Evidências](evidencias.md)
- [Demonstração](demo.md), [Reprodução](reproducao.md)
- [Recursos visuais](visuais.md)
- [Auditoria de visualizações interativas](visualizacoes-interativas.md)


## Padrão editorial e evolução

- [Guia editorial e voz](editorial-voice.md): tom, estrutura, terminologia e rastreabilidade.
- [Plano de evolução](maturity-roadmap.md): prioridades P0, P1 e P2 com critérios de aceite.

A documentação deve manter a distinção entre comportamento implementado, evidência observada, especificação arquitetural, simulação e proposta futura.
