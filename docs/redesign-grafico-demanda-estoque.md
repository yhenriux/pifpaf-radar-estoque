# Redesign do gráfico de demanda e estoque

## Decisão semântica

O gráfico não compara demanda diária com estoque total. A visualização usa duas séries com o mesmo eixo de unidades:

- **Demanda acumulada prevista:** soma da demanda diária prevista ao longo do horizonte.
- **Estoque disponível projetado:** saldo inicial menos a demanda acumulada prevista.

No cenário do pão de queijo de 1 kg no CD A, o saldo parte de 1.200 unidades e a demanda acumulada chega a 935 unidades no último ponto disponível. A cobertura permanece acima do horizonte de 14 dias neste recorte; nenhuma data de ruptura é inventada.

## Interações

O componente publicado no S01 possui:

- eixos numéricos e temporais;
- grade horizontal discreta;
- tooltip com data, produto, CD, demanda acumulada e estoque projetado;
- linha-guia no ponto em foco;
- foco por teclado;
- legenda para ocultar e exibir séries;
- zoom horizontal visual e restauração;
- indicadores de estoque atual, demanda acumulada e cobertura;
- texto alternativo e descrição textual equivalente.

## Estados considerados

O componente deve manter uma mensagem de dados insuficientes quando a série não tiver pontos. Valores nulos não devem gerar linhas artificiais. Estoque zerado, demanda zerada, ruptura antes do horizonte e ruptura após o horizonte devem ser calculados a partir da série e documentados com sua regra.

## Verificação

- node --check dist/script.js executado com sucesso.
- Publicação validada na versão 33.
- URL pública: https://radar-estoque-validade-pifpaf.yhenri-ux.chatgpt.site/#/visao-geral

A implementação usa SVG controlado pelo estado da interface, sem dependência adicional de biblioteca. Plotly ou ECharts continuam alternativas para séries maiores, exportação avançada ou zoom contínuo.
