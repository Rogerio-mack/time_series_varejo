# Séries Temporais do Varejo

## Resumo

Aqui são empregados e analisados modelos estatísticos (SARIMA) e de aprendizado de máquina (XGBOOST) para a predição de receitas futuras de uma grande varejista. O objetivo é buscar as melhores previsões para o próximo mês, e próximos 3 meses, ao longo de todo o ano. São empregadas inicialmente a série de receita total e, em seguida, o mesmo método é aplicado a 14 diferentes categorias de produtos (material-escolar, brinquedo, calçado, acessório, pet etc.) que compõe a receita total. Alguns dos principais resultados encontram-se a seguir e mais detalhes podem ser encontrados nos notebooks.

## Dados

São empregados séries de demanda e preços mensais de janeiro de 2021 a junho de 2024, em um total de 42 valores por série (total e para as 15 categorias de produtos).

<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/dados.png?raw=true" width="840">
<br>

## [Predições de Receita total](https://colab.research.google.com/github/Rogerio-mack/time_series_varejo/blob/main/timeseries_receita_total.ipynb)

### Modelo SARIMA 1M
<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/sarima_total.png?raw=true" width="840">
<br>

### Modelo XGBoost 1M
<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/xgboost_total.png?raw=true" width="840">
<br>

### Melhor Modelo 1M
<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/melhor_total.png?raw=true" width="640">
<br>
<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/melhor_total2.png?raw=true" width="640">
<br>

## [Predições de Receita por categoria](https://colab.research.google.com/github/Rogerio-mack/time_series_varejo/blob/main/timeseries_receitas_por_categoria.ipynb)

### Modelo SARIMA 1M
<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/sarima_categorias.png?raw=true" width="740">
<br>

### Modelo XGBoost 1M
<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/xgboost_categorias.png?raw=true" width="740">
<br>

### Melhores Modelos 1M e 3M
<br>
<img src="https://github.com/Rogerio-mack/time_series_varejo/blob/main/figures/melhor_categorias.png?raw=true" width="740">
<br>

## Conclusão

Séries de varejo são bastante desafiadoras pois incorparam variações de demanda, preços, troca de produtos etc. Apesar disso, os modelos obtidos fornecem uma estimativa, ao menos para metade dos produtos e incluindo receita total, útil diante da grande volatilidade que as séries apresentam, estando o resultado dos mdoelos estatísticos muito próximo dos obtidos pelos modelos de ML.

## Referências

[1] Oliveira, R., Abarracin, O. Y. E., Silva, G. R. (2024) **Introdução às Séries Temporais: Uma Abordagem Prática em Python**. Editora Mackenzie.

