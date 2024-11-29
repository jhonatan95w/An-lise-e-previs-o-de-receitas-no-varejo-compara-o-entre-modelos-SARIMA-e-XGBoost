# Análise e previsão de receitas no varejo: Comparação entre modelos SARIMA e XGBoost

## Resumo

Aqui, aplicamos e analisamos modelos estatísticos (SARIMA) e de aprendizado de máquina (XGBoost) para prever as receitas futuras de uma loja no setor de varejo. O objetivo é identificar os melhores modelos para prever as receitas tanto do próximo mês quanto dos três meses subsequentes, ao longo do ano.

A análise começa com a série de receita total da loja e, em seguida, é estendida para 14 categorias de produtos distintas (como material escolar, brinquedos, calçados, acessórios, pet, entre outras), que compõem a receita total. A aplicação dos modelos é feita com o intuito de entender as tendências e padrões das receitas de cada categoria, a fim de proporcionar previsões mais precisas e úteis.

Os principais resultados obtidos estão apresentados a seguir, e mais detalhes sobre a implementação e a metodologia podem ser encontrados nos notebooks utilizados para a análise.

## Dados
São empregados séries de demanda e preços mensais de janeiro de 2021 a junho de 2024, em um total de 42 valores por série (total e para as 15 categorias de produtos).
<div style="display: flex; justify-content: space-between;">
  <img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/e8a725030a39dd8e2ec3256d9f9c16fd91a64ff5/Images/Dados_ReceitaTotal.png" width="200">
  <img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/a012796bee12cf7e4c6dd5c6d175321aa64b4dd0/Images/Grafico_ReceitaTotal.png" width="500">
</div>

### Categorias de produtos

<div style="display: flex; justify-content: space-between;">
  <img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/6d4be082b6225f7d60975c7f2400c1d1183ff0fb/Images/categoriaProduto.png">
</div>

## [Predições de Receita total](//github.com/jhonatan95w/SeriesTemporais-Varejo/blob/main/SeriesTemporais_ReceitaTotal.ipynb)

### Modelo SARIMA 1M
<br>
<img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/6d4be082b6225f7d60975c7f2400c1d1183ff0fb/Images/Sarima1M_receitaTotal.png">
<br>

### Modelo XGBoost 1M
<br>
<img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/6d4be082b6225f7d60975c7f2400c1d1183ff0fb/Images/Xgboot1M_receitaTotal.png">
<br>

### Melhor Modelo 1M
<br>
<img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/6d4be082b6225f7d60975c7f2400c1d1183ff0fb/Images/melhorModelo1M.png">
<br>

### Melhor Modelo 3M
<br>
<img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/6d4be082b6225f7d60975c7f2400c1d1183ff0fb/Images/melhorModelo3M.png">
<br>

## [Predições de Receita por categoria](https://github.com/jhonatan95w/SeriesTemporais-Varejo/blob/main/SeriesTemporais_Categoria.ipynb)

### Modelo SARIMA 1M
<br>
<img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/6d4be082b6225f7d60975c7f2400c1d1183ff0fb/Images/Sarima1M_categorias.png">
<br>

### Modelo XGBoost 1M
<br>
<img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/6d4be082b6225f7d60975c7f2400c1d1183ff0fb/Images/XGBoost1M_categorias.png">
<br>

### Melhores Modelos 1M e 3M
<br>
<img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/934c1c1473371aa2d1b553822fadc3bd30650465/Images/melhoresModelo1M_3M.png">
<br>

## Conclusão

Séries de varejo são bastante desafiadoras pois incorparam variações de demanda, preços, troca de produtos etc. Apesar disso, os modelos obtidos fornecem uma estimativa, ao menos para metade dos produtos e incluindo receita total, útil diante da grande volatilidade que as séries apresentam, estando o resultado dos mdoelos estatísticos muito próximo dos obtidos pelos modelos de ML.

## Referências
