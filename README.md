# Análise da Inflação (IPCA) e Taxa de Desemprego no Brasil

## Coleta de Dados
Os dados foram coletados a partir da API do IBGE:
- **IPCA (Índice Nacional de Preços ao Consumidor Amplo)**: Dados mensais de inflação.
- **Taxa de Desemprego**: Dados mensais da taxa de desemprego.

## Tratamento de Dados
### IPCA
1. Renomeação das colunas para melhor compreensão (`V` para `ipca` e `D3C` para `data`).
2. Filtragem de valores inválidos e conversão do campo `data` para o formato de data e `ipca` para float.
3. Seleção de dados a partir de janeiro de 2004.

### Taxa de Desemprego
1. Renomeação das colunas (`V` para `desemprego` e `D3C` para `data`).
2. Filtragem de valores inválidos e conversão do campo `data` para o formato de data e `desemprego` para float.

### Cruzamento das Tabelas
- Junção dos dados de IPCA e desemprego usando a coluna `data`.

## Análise de Dados
### Comportamento da Inflação no Brasil
- Um gráfico de linha foi plotado para visualizar o comportamento do IPCA ao longo do tempo, revelando as flutuações da inflação desde 2004.

### Períodos com Maiores e Menores Taxas de Inflação
- Os períodos com as maiores e menores taxas de inflação foram identificados, destacando os extremos inflacionários. Períodos de alta inflação podem estar correlacionados com eventos econômicos ou políticos específicos.

### Valor Médio da Inflação
- As estatísticas descritivas da inflação (IPCA) foram calculadas, fornecendo uma visão geral da distribuição e centralidade dos valores de inflação ao longo do tempo.

### Relação entre Desemprego e Inflação
- Um modelo de regressão linear foi ajustado para entender a relação entre o desemprego e a inflação.
- Gráficos de dispersão com linhas de regressão foram utilizados para visualizar essa relação.

## Insights Obtidos
### Comportamento do IPCA
- Observou-se que a inflação no Brasil apresentou variações significativas ao longo do tempo. Períodos de alta inflação podem estar associados a crises econômicas, alterações nas políticas monetárias e eventos internacionais. Por exemplo, momentos de instabilidade política ou choques externos, como variações nos preços do petróleo, tendem a influenciar drasticamente a inflação.

### Períodos Extremamente Inflacionários
- A análise identificou meses com as maiores e menores taxas de inflação. Estes períodos são cruciais para entender a volatilidade da economia brasileira e os fatores que influenciam esses picos inflacionários. Períodos de inflação extrema podem ser causados por políticas fiscais e monetárias desajustadas, crises cambiais, ou ainda, por pressões de demanda e oferta. Identificar esses picos permite que políticas econômicas mais eficazes sejam desenhadas para mitigar tais eventos no futuro.

### Média da Inflação
- A análise das estatísticas descritivas revelou a média da inflação, bem como a variação e a dispersão dos valores de IPCA ao longo do tempo. Esses dados são essenciais para avaliar a estabilidade econômica e a eficiência das políticas monetárias adotadas. Uma inflação média controlada indica uma economia mais previsível e menos suscetível a choques externos.

### Relação entre Desemprego e Inflação
- A análise de regressão linear mostrou que existe uma relação entre a taxa de desemprego e a inflação. A linha de regressão indica uma correlação negativa entre essas variáveis, sugerindo que, em alguns períodos, uma menor taxa de desemprego está associada a uma maior inflação. Este padrão é consistente com a teoria econômica da Curva de Phillips, que sugere uma relação inversa entre desemprego e inflação no curto prazo. No entanto, a correlação observada não é determinística, ou seja, outros fatores macroeconômicos, como políticas fiscais, nível de investimento estrangeiro e a confiança do consumidor, também desempenham um papel crucial nesta dinâmica. É importante considerar esses fatores adicionais para um entendimento mais abrangente da economia. 
