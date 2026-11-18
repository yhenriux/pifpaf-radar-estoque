# Evidências da versão 45

A revisão do Sites é `bef04f206a2c084f073d6a9402e2cad87f811f73`. A URL pública respondeu HTTP 200 sem autenticação. O HTML servido contém a semente `572931` e a implementação da ficha de lote junto à linha selecionada.

| Capacidade | Evidência nesta revisão | Limite |
| --- | --- | --- |
| Indicadores e alertas | Funções do HTML executadas em Node reproduziram 410.188 unidades em risco de vencimento, 32.134 de ruptura e 158 alertas no recorte padrão | Base sintética com data fixa |
| Qualidade | 66.240 válidos de 66.271 recebidos, com 11 duplicidades, 13 validades ausentes e 7 saldos inválidos | Validação de amostra em memória |
| Lote e projeção | Contagem e pão de queijo de 1 kg reproduziram 11.698 unidades disponíveis e demanda de 3.576 em 14 dias | Projeção determinística |
| Ficha de lote | Teste de renderização abriu a ficha do lote correto e confirmou que ela desaparece ao limpar a seleção | O teste roda sem navegador |
| Navegação, gráficos e simulador | Comportamentos conferidos no HTML | Testes completos de teclado, acessibilidade e navegador continuam pendentes |

## Reprodução na interface

1. Abra o painel e use **Limpar filtros**. Compare os quatro cartões com o README.
2. Abra a central e confira os 158 alertas. Selecione Contagem, pão de queijo de 1 kg e 14 dias para conferir os valores da projeção.
3. Abra **Lotes e validade**. Clique em **Detalhes** em um lote e confira produto, lote, centro, validade e saldos. Use **Fechar detalhes** para recolher.
4. Abra o simulador. Compare um cenário dentro dos limites com outro de mesma origem e destino, que deve aparecer como inelegível.

[Abrir a versão publicada](https://radar-estoque-validade-pifpaf.yhenri-ux.chatgpt.site/#/painel)
