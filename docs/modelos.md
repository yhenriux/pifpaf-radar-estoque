# Projeções e simulador

A série diária vem de uma fórmula determinística com valores por produto e centro, ajuste semanal e termo senoidal. O histórico sintético usa a mesma função de geração. O HTML não treina um modelo nem executa backtesting. A faixa de ±17% em torno da demanda acumulada é uma heurística visual.

O saldo projetado começa no disponível e atende a demanda priorizando os lotes que vencem primeiro. O cálculo remove sobras vencidas e acumula a demanda não atendida. A projeção usa 7, 14 ou 21 dias contados a partir do dia seguinte à referência.

O simulador calcula uma transferência hipotética. Exige origem e destino distintos, quantidade inteira positiva limitada pela sobra em risco na origem e pela falta no destino, trânsito inteiro positivo e ao menos sete dias de validade na chegada, usando o primeiro vencimento da origem. Custos e margem informados devem ser finitos e não negativos.

**Benefício líquido estimado** = unidades com perda evitada × custo unitário evitável + unidades de ruptura cobertas × margem unitária − frete − R$ 67 de manuseio. O resultado depende das premissas inseridas. O cálculo ocorre no navegador e encerra na análise de cenário. Registro e execução pertencem à jornada anterior, em separado.
