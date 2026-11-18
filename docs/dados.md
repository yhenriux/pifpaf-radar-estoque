# Dados e indicadores

A amostra fixa de 16/11/2026 usa a semente `572931`. São 20 produtos e nove centros hipotéticos em Minas Gerais: Contagem, Betim, Ribeirão das Neves, Santa Luzia, Ibirité, Sabará, Nova Lima, Vespasiano e Sete Lagoas.

| Conjunto | Granularidade | Volume |
| --- | --- | ---: |
| Vendas sintéticas | Produto, centro e dia | 65.700 em 365 dias |
| Lotes válidos | Produto, centro e lote | 540, três por combinação |
| Entradas consideradas na qualidade | Vendas e lotes brutos | 66.271 |
| Válidos | Vendas geradas e lotes aprovados | 66.240 |
| Rejeitados | Ocorrências em lotes | 31 |

A validação identifica 11 duplicatas pela chave produto, centro, lote e data de referência, 13 registros sem validade e 7 saldos inválidos. O CSV exporta os lotes do recorte de centro e produto, com código, nome, centro, lote, saldo físico, reservas, disponibilidade e validade.

| Indicador | Regra |
| --- | --- |
| Disponível | Físico menos reservado |
| Vencimento em risco | Sobra disponível após o consumo projetado até o vencimento, no horizonte |
| Ruptura projetada | Demanda acumulada que ficou sem estoque para atendê-la |
| CDs com risco | Centros distintos com vencimento ou ruptura no recorte |
| Qualidade | Válidos ÷ recebidos, sobre a base geral |

Em Contagem, o pão de queijo de 1 kg tem 4.013, 5.001 e 3.003 unidades físicas. As reservas são 141, 103 e 75. O total disponível é 11.698. No horizonte padrão, a demanda acumulada desse recorte é 3.576. Em Betim, a ruptura projetada do mesmo produto é de 992 unidades.

A lista gera até dois alertas por produto e centro, um por tipo de risco positivo. Ordena por volume dividido por prazo mais um. As faixas alta e média começam em 100 e 33. Para vencimento, o prazo mostrado usa o primeiro lote. Para ruptura, usa o horizonte, sem indicar o primeiro dia exato da falta.
