# Análise Exploratória de Dados: Covid-19
 <img src="images/project1_2.jpeg" alt="Uma bela paisagem" width="900" height="500" title="Clique para ampliar">

 <h2>1. Introdução</h2>

<h3><strong>1.1. TLDR</strong></h3>

<ul>
  <li><strong>Dashboard</strong>:
    <ul>
      <li>Google Data Studio <a href="https://lookerstudio.google.com/reporting/08819073-431e-4f2a-b594-16c02177d8a8">link</a></li>
    </ul>
  </li>
  <li><strong>Processamento</strong>:
    <ul>
      <li>Kaggle Notebook <a href="https://www.kaggle.com/fabiopereira445/projeto-ebac-covid19">link</a></li>
    </ul>
  </li>
  <li><strong>Fontes</strong>:
    <ul>
      <li>Casos pela universidade John Hopkins <a href="https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports">link</a></li>
      <li>Vacinação pela universidade de Oxford <a href="https://covid.ourworldindata.org/data/owid-covid-data.csv">link</a></li>
    </ul>
  </li>
</ul>
 <h3> 1.2 Metas e objetivos</h3>
 <p>O objetivo principal do projeto é fornecer uma compreensão detalhada do impacto da pandemia no país até 30 de dezembro de 2021, destacando áreas críticas que precisam de intervenção e estratégias recomendadas para mitigar a disseminação do vírus.
</p>
<h3><strong>1.3. Pandemia Coronavírus 2019</strong></h3>

<blockquote>
  <p>A COVID-19 é uma infecção respiratória aguda causada pelo coronavírus SARS-CoV-2, potencialmente grave, de elevada transmissibilidade e de distribuição global. Fonte: Governo brasileiro <a href="https://www.gov.br/saude/pt-br/coronavirus/o-que-e-o-coronavirus">link</a>.</p>
</blockquote>

<p>A disponibilidade de dados sobre a evolução da pandemia no tempo em uma determinada região geográfica é fundamental para o seu combate! Este projeto busca construir um dashboard de dados para exploração e visualização interativa de dados sobre o avanço de casos e da vacinação do Brasil. O processamento de dados está neste <a href="https://www.kaggle.com/fabiopereira445/projeto-ebac-covid19">link</a> e o dashboard, neste <a href="https://lookerstudio.google.com/reporting/08819073-431e-4f2a-b594-16c02177d8a8">link</a>.</p>
 <h2>2.0. Dados</h2>
    </ul>
     <p><strong>Os dados sobre casos</strong> da COVID-19 são compilados pelo centro de ciência de sistemas e engenharia da universidade americana John Hopkins (<a href=" https://www.jhu.edu">link</a>). Os dados são atualizados diariamente deste janeiro de 2020 com uma granularidade temporal de dias e geográfica de regiões de países (estados, condados, etc.). O website do projeto pode ser acessado neste <a href="https://systems.jhu.edu/research/public-health/ncov/">link</a> enquanto os dados, neste <a href="https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports       ">link</a>. Abaixo estão descritos os dados derivados do seu processamento.</p>
    <ul>
    <ul>
        <li>date: data de referência;</li>
        <li>state: estado;</li>
        <li>country: país;</li>
        <li>population: população estimada;</li>
        <li>confirmed: número acumulado de infectados;</li>
        <li>confirmed_1d: número diário de infectados;</li>
        <li>confirmed_moving_avg_7d: média móvel de 7 dias do número diário de infectados;</li>
        <li>confirmed_moving_avg_7d_rate_14d: média móvel de 7 dias dividido pela média móvel de 7 dias de 14 dias atrás;</li>
        <li>deaths: número acumulado de mortos;</li>
        <li>deaths_1d: número diário de mortos;</li>
        <li>deaths_moving_avg_7d: média móvel de 7 dias do número diário de mortos;</li>
        <li>deaths_moving_avg_7d_rate_14d: média móvel de 7 dias dividido pela média móvel de 7 dias de 14 dias atrás;</li>
        <li>month: mês de referência;</li>
        <li>year: ano de referência.</li>
    </ul>
      </ul>
    <p><strong>Os dados sobre vacinação</strong> da COVID-19 são compilados pelo projeto Nosso Mundo em Dados (Our World in Data ou OWID) da universidade britânica de Oxford (<a href="https://www.ox.ac.uk">link</a>). Os dados são atualizados diariamente deste janeiro de 2020 com uma granularidade temporal de dias e geográfica de países. O website do projeto pode ser acessado neste <a href="https://ourworldindata.org">link</a> enquanto os dados, neste <a href="https://covid.ourworldindata.org/data/owid-covid-data.csv ">link</a>. Abaixo estão descritos os dados derivados do seu processamento.</p>
    <ul>
    <ul>
        <li>date: data de referência;</li>
        <li>country: país;</li>
        <li>population: população estimada;</li>
        <li>total: número acumulado de doses administradas;</li>
        <li>one_shot: número acumulado de pessoas com uma dose;</li>
        <li>one_shot_perc: número acumulado relativo de pessoas com uma dose;</li>
        <li>two_shots: número acumulado de pessoas com duas doses;</li>
        <li>two_shot_perc: número acumulado relativo de pessoas com duas doses;</li>
        <li>three_shots: número acumulado de pessoas com três doses;</li>
        <li>three_shot_perc: número acumulado relativo de pessoas com três doses;</li>
        <li>month: mês de referência;</li>
        <li>year: ano de referência.</li>
    </ul>
<h2>3.0 Ferramentas utilizadas</h2>
<img src="images/img_python.svg" alt="Uma bela paisagem" width="75" height="25" title="img_python">
<img src="images/img_VScode.svg" alt="Uma bela paisagem" width="75" height="25" title="img_VScode">
<img src="images/img_jupyter.svg" alt="Uma bela paisagem" width="75" height="25" title="img_jupyter">
<h3>3.1 Bibliotecas Python utilizadas</h3>
<h4> Manipulação de dados</h4>
<img src="images/img_pandas.svg" alt="Uma bela paisagem" width="75" height="25" title="img_pandas">
<img src="images/img_numpy.svg" alt="Uma bela paisagem" width="75" height="25" title="img_numpy">
<img src="images/img_geopandas.png" alt="Uma bela paisagem" width="75" height="25" title="img_numpy">
<h4> EDA</h4>
<img src="images/img_matplotlib.svg" alt="Uma bela paisagem" width="75" height="25" title="img_matplotlib">
<img src="images/img_seaborn.svg" alt="Uma bela paisagem" width="75" height="25" title="Clique para ampliar">

<h2>4.0 Exploratory Data Analysis</h2>
 <img src="figures/plot1.png" alt="Uma bela paisagem" width="1000" height="500" title="figura 1">
 <P><b>Insight</b></p> <P>O gráfico fornece uma visão geral . <P>
  <img src="figures/plot2.png" alt="Uma bela paisagem" width="1000" height="500" title="figura 2">
   <P><b>Insight</b></p>Desigualdade na Demanda: .<P>
   <img src="figures/plot3.png" alt="Uma bela paisagem" width="1000" height="500" title="figura 3">
    <P><b>Insight</b></p>Dominância de Brasília e Taguatinga:<P>
    <img src="figures/plot4.png" alt="Uma bela paisagem" width="1000" height="500" title="figura 4">
   <P><b>Insight</b></p>A concentração das entregas.<P>
     <img src="figures/plot5.png" alt="Uma bela paisagem" width="1000" height="1650" title="figura 5">
     <P><b>Insight</b></p>Concentração em Poucas Áreas:<P>

</body>
</html>
