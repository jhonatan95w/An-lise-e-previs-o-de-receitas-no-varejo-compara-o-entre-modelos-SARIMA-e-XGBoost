# Análise e previsão de receitas no varejo: Comparação entre modelos SARIMA e XGBoost

## Resumo

Aqui, aplicamos e analisamos modelos estatísticos (SARIMA) e de aprendizado de máquina (XGBoost) para prever as receitas futuras de uma loja no setor de varejo. O objetivo é identificar os melhores modelos para prever as receitas tanto do próximo mês quanto dos três meses subsequentes, ao longo do ano.

A análise começa com a série de receita total da loja e, em seguida, é estendida para 14 categorias de produtos distintas (como material escolar, brinquedos, calçados, acessórios, pet, entre outras), que compõem a receita total. A aplicação dos modelos é feita com o intuito de entender as tendências e padrões das receitas de cada categoria, a fim de proporcionar previsões mais precisas e úteis.

Os principais resultados obtidos estão apresentados a seguir, e mais detalhes sobre a implementação e a metodologia podem ser encontrados nos notebooks utilizados para a análise.

## Dados
São empregados séries de demanda e preços mensais de janeiro de 2021 a junho de 2024, em um total de 42 valores por série (total e para as 15 categorias de produtos).
<div style="display: flex; justify-content: space-between;">
  <img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/e8a725030a39dd8e2ec3256d9f9c16fd91a64ff5/Images/Dados_ReceitaTotal.png" width="200">
  <img src="https://raw.githubusercontent.com/jhonatan95w/SeriesTemporais-Varejo/a012796bee12cf7e4c6dd5c6d175321aa64b4dd0/Images/Grafico_ReceitaTotal.png" width="800">
</div>
