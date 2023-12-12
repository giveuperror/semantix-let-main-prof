# Análise de Poluentes no Estado de São Paulo

## Introdução

Este repositório apresenta uma análise abrangente dos dados de poluição atmosférica no estado de São Paulo. Os dados abordam uma variedade de informações, incluindo data, hora, local de medição, tipos de poluentes e concentrações medidas.

## Coleta de Dados

### Visão Geral
Os dados foram coletados ao longo de um período extenso, iniciando em 01:00 de 01/01/2015 e encerrando em 24:00 de 31/12/2021. O conjunto de dados contém 2557 datas distintas, cobrindo um intervalo de 7 anos, com um ano bissexto incluso.

### Estrutura do DataFrame
O dataframe contém informações detalhadas sobre cada medição, incluindo ID, Data, Hora, Estação, Código, Poluente, Valor, Unidade e Tipo de medição.

## Modelagem

### Distribuição das Medições
A distribuição das medições revela uma variedade de padrões ao longo do dia, evidenciados por um histograma. Valores extremos identificados no boxplot apontam para a presença de outliers discrepantes.

### Métodos de Medição
99.9% das medições foram realizadas automaticamente, enquanto 43 locais tiveram medições manuais.

### Estatísticas das Concentrações
- Desvio-padrão elevado (250), indicando alta dispersão.
- Concentração majoritária em intervalos menores ($<=45 \frac{\mu g}{m^{3}}$).
- Outliers extremos afetando a distribuição geral dos dados.

### Correlação (Hora x Concentração) por Poluente
Os coeficientes de correlação entre a hora do dia e a concentração de cada poluente variam significativamente:

- MP10: ~0.005
- O3: ~0.19
- NO2: ~0.12
- CO: ~0.9
- MP2.5: -0.001
- SO2: -0.025
- NO: -0.10

Os poluentes 'FMC' e 'PTS' foram excluídos da análise devido à ausência de variação na hora de medição.

## Conclusões

### Locais Críticos de Poluição
Identificamos locais críticos que demandam ações imediatas para reduzir a poluição, incluindo:
- Araraquara
- Araçatuba
- Cubatão - Centro
- Cubatão - Vale do Mogi
- Cubatão - Vila Parisi
- Guarulhos - Pimentas
- Marília
- Paulínia - Sul
- Presidente Prudente
- Ribeirão Preto
- Santa Gertrudes
- Cid.Universitária USP - IPEN
- Grajaú - Parelheiros
- Osasco
- Perus
- Pico do Jaraguá
- Rio Claro - Jardim Guanabara
- São José do Rio Preto

### Evolução Temporal dos Poluentes
A análise permitiu observar a evolução das concentrações de poluentes ao longo do tempo em cada local, possibilitando associações com fatores históricos locais, como tráfego veicular e atividades industriais.

### Papel da Análise de Dados
Esta análise demonstra como a análise de dados pode fornecer insights valiosos para orientar ações e políticas públicas. A compreensão das relações entre variáveis é fundamental para abordar questões complexas como a poluição atmosférica.

## Considerações Finais

Esta análise fornece uma visão abrangente da situação dos poluentes no estado de São Paulo, evidenciando a importância da análise de dados na tomada de decisões estratégicas e ações corretivas.
