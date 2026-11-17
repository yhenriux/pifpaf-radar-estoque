# Evidências, proveniência e limites de validação

**Atualização inicial:** 17/11/2026.

## Fontes analisadas

1. **Repositório GitHub** `yhenriux/pifpaf-radar-estoque`: encontrado **público e vazio** antes desta documentação; código-fonte não inspecionável.
2. **Blueprint da conversa** `JORNADAS_E_TELAS.md`, `radar-fluxos-telas.json` e `AGENTS.md`: contém 19 telas, cinco jornadas, recorte de dados e arquitetura proposta.
3. **Aplicação pública** [radar-estoque-validade-pifpaf.yhenri-ux.chatgpt.site](https://radar-estoque-validade-pifpaf.yhenri-ux.chatgpt.site/): inspeção textual de página inicial exibiu navegação por módulos, seleção de perfil, cenário de pão de queijo e mensagem de dados sintéticos. Isso **não verifica código, API, persistência, login anônimo ou todas as rotas**.
4. **Capturas de interface** fornecidas pelo responsável: referências visuais da marca corporativa Pif Paf Alimentos e versões do Radar.

## Matriz de estado

| Item | Evidência disponível | Classificação |
|---|---|---|
| URL pública responde com conteúdo | Leitura de aba da aplicação | Observado em sessão; anonimato não testado |
| Interface com navegação por módulos | Texto da aba inicial | Observado parcialmente |
| 19 telas e cinco jornadas | Blueprint | Especificado |
| Dados sintéticos: 20 SKUs, 2 CDs, 12 meses | Blueprint | Especificado |
| FastAPI, Python, ETL/ELT | Blueprint | Proposto, código não auditado |
| DuckDB, Azure SQL e Azure Blob | Blueprint | Alternativas, implantação não confirmada |
| scikit-learn, MLflow, backtesting | Blueprint | Proposto, não auditado |
| Tableau e Power BI | Plano de demonstração | Integrações reais não verificadas |
| Cálculo econômico | Regra descrita | Fórmulas exigem teste com código |
| Testes E2E e CI | Plano de trabalho | Não comprovados |
| Identidade visual Pif Paf Alimentos | Material público/capturas | Referência, sem homologação da empresa |

## Critérios de afirmação

- **Observado:** existe uma evidência acessível e identificada.
- **Especificado:** documentação descreve o comportamento esperado.
- **Implementado:** código, build ou endpoint verificado.
- **Testado:** execução registrada, com entradas e saídas.
- **Operacional:** sistema conectado a fontes reais com autorização e supervisão.

Nunca promover um item para estágio superior sem evidência.

## Transparência dos resultados

Todo ganho econômico do case é **simulado/projetado**. Não atribuir economias realizadas à Pif Paf Alimentos; não interpretar imagens demonstrativas como comprovação de infraestrutura nem inferir vínculo comercial ou implantação.
