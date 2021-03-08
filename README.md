# Prevendo o comportamento da COVID-19 com Evolução Diferencial e um modelo tipo Maxwell-Boltzmann

  *Analysis of time series datasets of recorded cases and deaths from COVID-19 and recorded cases and deaths from SARS (severe acute respiratory syndrome) in Brazil using Differential Evolution and a combination model of "Maxwell-Boltzmann-like" distributions to forecast the behavior of the first and second wave of COVID-19 in Brazil.*

  Análise de datasets contendo séries temporais de casos e óbitos por COVID-10 registrados e casos e óbitos por SRAG (síndrome respiratória aguda grave) no Brazil utilizando Evolução Diferencial e um modelo combinatório de distribuições tipo Maxwell-Boltzmann para prever o comportamento da primeira e segunda onda de COVID-19 no Brazil.

 

## Sobre ED, Distribuição de Maxwell-Boltzmann e COVID-19:

 Evolução Diferencial é um algorítmo evolutivo simples da categoria de algorítmos meta-heurísticos, que através da criação de populações de soluções, suas seleções e recombinações, é capaz de obter um solução ótima ou aproximadamente ótima para um problema.
 
 Desde que tenhamos dados o suficiente é possível, facilmente, utilizar Evolução Diferencial (Autoadaptativa ou não) para ajustar curvas/séries temporais provenientes de fenômenos físicos, por exemplo. Assim, podemos ajustar curvas geradas por fenômenos antropológicos como os relacionados ao COVID-19, desde que escolhamos um modelo matemáticos conveniente, que possa ser ajustado aos dados.

 A equação de densidade de frequência relativa (distribuição de velocidades de Maxwell-Boltzmann) é um modelo matemático utilizado para determinar a distruibuição de velocidades de moléculas contidas em um gás ideal:
 
 <p align="center">
 <img src="eqs_png/eq_max_bol.png" align=middle/>
 </p>
 
 Dependendo dos parâmetros escolhido massa *m* e temperatura *T*, a função pode esboçar uma clara distruibuição assimétrica (se comparada com uma distruibuição de Gauss) que pode ser capaz de ajustar os dados provenientes da pandemia de COVID-19 no Brasil se associada a um conveniente algoritmo de otimização, já que a distruibuição é capaz de esboçar uma subida abrupta e um comportamento de cauda. 
 
 Assim, foi contruído o seguinte modelo:

 <p align="center">
 <img src="eqs_png/eq_waves.png" align=middle/>
 </p>
 
 Onde:
 
 <p align="center">
 <img src="eqs_png/eq_wave_1.png" align=middle/>
 </p>
 
 e
 
 <p align="center">
 <img src="eqs_png/eq_wave_2.png" align=middle/>
 </p>
 
## Testando o modelo tipo Maxwell-Boltzmann:


E encontrar os parâmeros que melhor ajustam a curva do modelo aos devidos dados utilizando Evolução Diferencial como algoritmo de otimização.


## Ajustando casos de COVID-19:
 
 Ajuste feito em 03/01/2021 (Média dos parâmetros de 20 runs do algoritmo de ED):
 
 <p align="center">
 <img src="casos_covid_ajuste.png" align=middle/>
 </p>
 
 
 Ajuste atualizado em 03/03/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):
 
 <p align="center">
 <img src="update_03_03_2021/casos_covid_ajuste_03_03_2021.png" align=middle/>
 </p>
 
 Previsão dos próximos dias epidemiológicos feita em 03/01/2021 (Média dos parâmetros de 20 runs do algoritmo de ED):
 
 <p align="center">
 <img src="casos_covid_previsao.png" align=middle/>
 </p>
 
 Previsão dos próximos dias epidemiológicos atualizada em 03/03/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):
 
 <p align="center">
 <img src="update_03_03_2021/casos_covid_previsao_03_03_2021.png" align=middle/>
 </p>

## Ajustando óbitos por COVID-19:

 Ajuste feito em 03/01/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):
 
 <p align="center">
 <img src="obitos_covid_ajuste.png" align=middle/>
 </p>
 
 Ajuste atualizado em 03/01/2021 (Média dos parâmetros de 20 runs do algoritmo de ED):
 
 <p align="center">
 <img src="update_03_03_2021/obitos_covid_ajuste_03_03_2021.png" align=middle/>
 </p>
 
 Previsão dos próximos dias epidemiológicos feita em 03/01/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):
 
 <p align="center">
 <img src="obitos_covid_previsao.png" align=middle/>
 </p>
 
 Previsão dos próximos dias epidemiológicos atualizada em 03/01/2021 (Média dos parâmetros de 20 runs do algoritmo de ED):
 
 <p align="center">
 <img src="update_03_03_2021/obitos_covid_previsao_03_03_2021.png" align=middle/>
 </p>

## Ajustando casos de SRAG:

 Uma forma de tentarmos prever o comportamento da segunda onda de COVID-19 é analisando os casos e óbitos por Síndrome Respiratória Aguda Grave, já que devido à subnotificação de casos e mortes no Brasil, é possível tentar estimar, por exemplo, óbitos subnotificados por COVID-19 através da análise dos dados de SRAG.

 Ajuste feito em 03/01/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):

 <p align="center">
 <img src="casos_srag_ajuste.png" align=middle/>
 </p>
 
 Ajuste atualizado em 03/03/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):

 <p align="center">
 <img src="update_03_03_2021/casos_srag_ajuste_03_03_2021.png" align=middle/>
 </p>
 
 Previsão dos próximos dias epidemiológicos feita em 03/01/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):
 
 <p align="center">
 <img src="casos_srag_previsao.png" align=middle/>
 </p>
 
 Previsão dos próximos dias epidemiológicos atualizado em 03/03/2021 (Média dos parâmetros de 10 runs do algoritmo de ED):
 
 <p align="center">
 <img src="update_03_03_2021/casos_srag_previsao_03_03_2021.png" align=middle/>
 </p>

## Ajustando óbitos por SRAG:
 
 Ajuste feito em 03/01/2021 (Média dos parâmetros de 5 runs do algoritmo de ED):
 
 <p align="center">
 <img src="obitos_srag_ajuste.png" align=middle/>
 </p>
 
 Ajuste atualizado em 03/03/2021 (Média dos parâmetros de 5 runs do algoritmo de ED):
 
 <p align="center">
 <img src="update_03_03_2021/obitos_srag_ajuste_03_03_2021.png" align=middle/>
 </p>
 
 Previsão dos próximos dias epidemiológicos feita em 03/01/2021 (Média dos parâmetros de 5 runs do algoritmo de ED):
 
 <p align="center">
 <img src="obitos_srag_previsao.png" align=middle/>
 </p>

 Previsão dos próximos dias epidemiológicos atualizada em 03/01/2021 (Média dos parâmetros de 5 runs do algoritmo de ED):
 
 <p align="center">
 <img src="update_03_03_2021/obitos_srag_previsao_03_03_2021.png" align=middle/>
 </p>

## Prevendo o pior momento da segunda onda de COVID-19 no Brasil:
 
 Para tentarmos visualizar o comportamento do auge da segunda onda de COVID-19 no Brasil podemos plotar as curvas correspondentes às gaussianas combinadas dos ajustes anteriores de forma normalizada:

 Normalizações feitas em 03/01/2021:

 <p align="center">
 <img src="normalizacoes.png" align=middle/>
 </p>
  
  Normalizações atualizadas em 03/03/2021:

 <p align="center">
 <img src="update_03_03_2021/normalizacoes_03_03_2021.png" align=middle/>
 </p>
  
  Em nosso modelo, o parâmetro &beta;<sub>i</sub> representa o centro do máximo de cada curva gaussiana, assim, podemos ver que, segundo nossa estimativa:
  
  Estimativas feitas em 03/01/2021:
  
  - 13 de abril (aproximadamente) será o dia com mais casos de COVID-19 registrados na segunda onda;
  - 12 de julho (aproximadamente) será o dia com mais óbitos por COVID-19 registrados na segunda onda;
  - 20 de março (aproximadamente) será o dia com mais casos de SRAG registrados na segunda onda;
  - 20 de maio (aproximadamente) será o dia com mais óbitos por SRAG registrados na segunda onda;
  - Em média, 9 de maio (aproximadamente) será o "pior dia" da segunda onda, considerando todos os fatores anteriores.
  
  
  Estimativas atualizadas em 03/03/2021:
  
  - 17 de fevereiro (aproximadamente) foi o dia com mais casos de COVID-19 registrados na segunda onda;
  - 19 de maio (aproximadamente) será o dia com mais óbitos por COVID-19 registrados na segunda onda;
  - 27 de abril (aproximadamente) será o dia com mais casos de SRAG registrados na segunda onda;
  - 22 de maio (aproximadamente) será o dia com mais óbitos por SRAG registrados na segunda onda;
  - Em média, 22 de abril (aproximadamente) será o "pior dia" da segunda onda, considerando todos os fatores anteriores.
  
  *OBS: Considerando 13 de março de 2020 como o primeiro dia epidemiológico do Brasil*
  
  ## Estas são boas previsões acerca da segunda onda de COVID-19 no Brasil?
  
  Não. O Teorema Central do Limite nos garante que a distribuição amostral, quando a amostra aumenta, se aproxima de uma distribuição normal, ou, distruibuição gaussiana. Dada a evolução dos pontos da série temporal proveniente dos dados gerados por fenômenos antropológicos e biológicos relacionados ao COVID-19, pode-se pensar que uma curva gaussina poderia ajustar muito bem estes pontos. Porém,  as variáveis do fenômeno que geram os respectivos dados não são independentes, desta forma, não podem ser aproximados facilmente por este tipo de função. Necessitaríamos de algo um pouco mais sofisticado, como uma gaussiana modificada, o que faria, por exemplo, que a curva ajustasse os pontos iniciais de nossos datasets, o que claramente não acontece em nosso casos, e pode ser visualizado nos gráficos.
  
  Outro aspecto a se atentar, é que talvez não tenhamos dados o suficiente da segunda onda para inferirmos um comportamento à longo prazo, principalmente nas previsões utilizando dados de SRAG, que parecem estar desatualizados e/ou subnotificados nos datasets investigados.
  
## Referências:

* **"MonitoraCovid-19"** https://bigdata-covid19.icict.fiocruz.br/; (Visualizado em: 03/01/2021 nos primeiros ajustes e 03/03/2021 nos ajustes maisrecentes) (Daqui foram obtidos os *datasets* utilizados.

* **"InfoGripe"** http://info.gripe.fiocruz.br/; (Visualizado em: 16/05/2020) (Onde os dados são divulgados originalmente. Daqui é possível obter *datasets* mais robustos com registros até o ano de 2009).
