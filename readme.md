# Análise Geoespacial do Município do Rio de Janeiro( alura )

Este projeto utiliza diversas bibliotecas de Python para realizar uma análise geoespacial no município do Rio de Janeiro. As bibliotecas utilizadas incluem `geopandas`, `pandas`, `numpy`, `seaborn` e `shapely`. Abaixo estão as instruções e explicações detalhadas sobre os passos realizados no código fornecido.

## Dados Utilizados
- * RJ_Municipios_2022.shp *: Arquivo shapefile contendo os limites dos municípios do Rio de Janeiro.
- dados.csv: Dados tabulares contendo informações geográficas.
- metro.geojson: Dados das linhas de metrô.
- trem.geojson: Dados das linhas de trem.
- brt.geojson: Dados das linhas de BRT.
- Cobertura_Vegetal_e_Uso_da_Terra_2018.geojson: Dados de cobertura vegetal e uso da terra, necessário baixar.

## Descrição do Processo
1. Carregamento dos Dados: Os dados geoespaciais e tabulares são carregados a partir das URLs fornecidas.
2. Filtragem e Conversão: Apenas o município do Rio de Janeiro e as praias são filtrados, e as coordenadas são convertidas para o sistema UTM.
3. Criação de GeoDataFrames: Pontos geométricos são criados a partir das coordenadas de longitude e latitude.
4. Filtragem Geoespacial: Os dados são filtrados para incluir apenas aqueles dentro dos limites do Rio de Janeiro.
5. Cálculo de Distâncias: Distâncias mínimas entre pontos de interesse (metrô e praias) são calculadas.
6. Análise e Visualização: Correlações entre variáveis numéricas são analisadas e visualizadas usando `seaborn`.