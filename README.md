# Análise e previsão de receitas no varejo: Comparação entre modelos SARIMA e XGBoost

Artigo:
- [Análise e previsão de receitas no varejo: comparação entre modelos SARIMA e XGBoost](https://github.com/jhonatan95w/SeriesTemporais-Varejo/blob/dc61e0850ec04dab6ae3ac8db05cdaaf5305f995/AnaliseSeriesTemporaisVarejo_ComparacoesSarimaXGBoost.pdf)

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

Este trabalho teve como objetivo analisar e prever as receitas mensais de diversas categorias do varejo utilizando os modelos SARIMA e XGBoost. Embora as séries de dados de varejo apresentem desafios devido à volatilidade e fatores externos, os modelos forneceram estimativas boas, especialmente para a receita total e categorias com padrões mais regulares. O modelo SARIMA se destacou nas previsões de curto prazo (1 mês), enquanto o XGBoost foi mais eficaz em horizontes maiores (3 meses), adaptando-se melhor a relações complexas nos dados. No entanto, algumas categorias, como Natal e Vestuário, apresentaram maiores dificuldades devido a fatores sazonais e externos. As limitações indicam a necessidade de ajustes nos modelos, como a inclusão de variáveis exógenas, para melhorar a precisão. Apesar disso, as previsões foram úteis para o planejamento de estoques e orçamentos. Futuros estudos podem explorar técnicas mais avançadas, como redes neurais, para aprimorar ainda mais as previsões em cenários mais complexos.

## Autores

- **Jhonatan Zhang Deng**  
- **Rogério de Oliveira** - *Orientador do projeto*

## Referências

[1] Santos, Angela Maria Medeiros Martins & Costa, Claudia Soares (1997). Características gerais do varejo no Brasil. BNDES. Banco Nacional de Desenvolvimento Econômico e Social.

[2] Botelho, Delane & Guissoni, Leandro (2016). Varejo: competitividade e inovação. Revista de Administração de Empresas, 56(6), 596-599. SciELO Brasil.

[3] de Oliveira, Rogério & Albarracín, Orlando YE & da Silva, Gustavo Rocha (2024). Introdução às Séries Temporais: Uma Abordagem Prática em Python. Github.

[4] Hyndman, RJ (2018). Forecasting: principles and practice (Capítulo [2.3]: Time series patterns). OTexts.

[5] Box, George EP & Jenkins, Gwilym M & Reinsel, Gregory C & Ljung, Greta M (2015). Time series analysis: forecasting and control. John Wiley & Sons.

[6] Chen, Tianqi & Guestrin, Carlos (2016). Xgboost: A scalable tree boosting system. Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, 785-794. Disponível em: https://dl.acm.org/doi/10.1145/2939672.2939785.

[7] Pinto, Ricardo Aurélio Quinhões et al. (2013). Gestão de estoque e lean manufacturing: estudo de caso em uma empresa metalúrgica. Revista Administração em Diálogo-RAD, 15(1).

[8] Holanda, Briana Maria Souza et al. (2022). Gestão e organização do estoque em empresas de varejo: um estudo comparativo de duas empresas de Loanda, Paraná. Desenvolve Revista de Gestão do Unilasalle, 11(3).

[9] Oliveira, Anderson dos Santos de et al. (2024). Análise comparativa de modelos de previsão para receitas correntes mensais do estado de Alagoas: abordagens econométricas e redes neurais. UFAL.

[10] Silveira, Ian Vieira et al. (2019). Modelo de previsão de demanda com o uso de aprendizado supervisionado de máquina: um estudo de caso em uma empresa de varejo. UFSC. Florianópolis, SC.

[11] Lima, José Eduardo Carvalho & de Castro, Lucas Ferreira & Cartaxo, Glauber Araujo Alencar (2019). Aplicação do modelo SARIMA na previsão de demanda no setor calçadista. ID on line. Revista de psicologia, 13(46), 892-913.

[12] Walter, Olga Maria Formigoni Carvalho & Henning, Elisa & Moro, Graciela & Samohyl, Robert Wayne (2013). Aplicação de um modelo SARIMA na previsão de vendas de motocicletas. Exacta, 11(1), 77-88. Universidade Nove de Julho.

[13] Divisekara, Roshani W & Jayasinghe, GJMSR & Kumari, KWSN (2020). Forecasting the red lentils commodity market price using SARIMA models. SN Business & Economics, 1(1), 20. Springer.

[14] Las Casas, Alexandre Luzzi & Garcia, Maria Tereza (2007). Estratégias de marketing para varejo. In Inovações e diferenciações estratégicas que fazem a diferença no marketing de varejo. São Paulo: Novatec.

[15] Scikit-learn (2024). Metrics and scoring: quantifying the quality of predictions. Disponível em: https://scikit-learn.org/1.5/modules/model_evaluation.html. Acesso em: 12 de novembro de 2024.

[16] Ryan Holbrook (2020). Time Series as Features. Disponível em: https://www.kaggle.com/code/ryanholbrook/time-series-as-features. Acesso em: 19 de novembro de 2024.

[17] Eda Kavlakoglu, Erika Russi (2024). O que é o XGBoost?. Disponível em: https://www.ibm.com/br-pt/topics/xgboost. Acesso em: 12 nov. 2024.

[18] Alexandre Zajic (2022). What Is Akaike Information Criterion (AIC)? Disponível em: https://builtin.com/data-science/what-is-aic. Acesso em: 19 nov. 2024.







