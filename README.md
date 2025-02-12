<h1>Projeto Competitivo de League of Legends</h1>
<hr>
Este projeto foi desenvolvido com o intuito de auxiliar apostadores na tomada de decisões melhores, afim de aumentar a probabilidade de acerto de suas apostas no competitivo de Esports do jogo League of Legends.

<h2><a href="https://app.powerbi.com/groups/me/reports/625b7afa-b96f-4607-a76b-a40f45ef04b4/b46cddca13a76096b92d?experience=power-bi"> Acesse o Dashboard aqui </a></h2>

<hr>
<br>

<h1>Entendendo a Base de Dados</h1>

<h2>Dados da partida:</h2>

Essa tabela exibe dados das partidas.

<b>MatchID</b> - Identificador exclusivo para todo o conjunto de correspondências

<b>matchType</b> - Tipo de competição

<b>conjunto de jogos</b> - Número específico da rodada do jogo

<b>MatchDate</b> - Data da partida

<br>

<h2>Dados do conjunto de jogos:</h2>

Essa tabela exibe dados dos jogos disputados.

<b>Duração</b> - Duração da rodada do jogo, formatada como "%m/%d/%yyyy"

<b>vitória</b> - Equipe vencedora

<br>

<h2>Dados da equipe:</h2>

Essa tabela exibe dados das equipes.

<b>TeamN_{Attributes}</b> -  Designação do time (1 representa o time da casa, 2 representa o time visitante)

<b>região</b> - Origem nacional ou regional da equipe

<b>Barão</b> - Número de mortes do Barão Nashor

<b>Dra</b> -  Número de mortes de dragões

<b>Torres</b> - Número de torres destruídas

<b>{Team}_banN</b> - Campeão banido na fase de banimento N

<br>

<h2>Dados do jogador:</h2>

Essa tabela exibe dados dos jogadores das equipes

<b>{Team}_playerN_{Atributos}</b> - Posição do jogador (1-TOP; 2-JUG; 3-MID; 4-ADC; 5-SUP)

<b>{Team}_{Player}_name</b> - Nome do jogador

<b>{Equipe}_{Jogador}_escolha</b> - Campeão selecionado

<b>{Equipe}_{Jogador}_K</b> - Mortes

<b>{Equipe}_{Jogador}_D</b> - Mortes

<b>{Time}_{Jogador}_A</b> - Assistências

<b>{Equipe}_{Jogador}_CS</b> - Pontuação de Creep (mortes de lacaios)

<b>{Team}_{Player}_gold</b> - Ouro ganho

<b>{Team}_{Player}_damage</b> - Dano causado

<b>{Team}_{Player}_tanking</b> - Dano recebido

<br>

<h4>Os seguintes (sub)conjuntos de dados fornecem insights abrangentes sobre estatísticas de partidas competitivas de League of Legends, derivados do conjunto de dados bruto original:</h4>

<b>team.csv</b> - Análise abrangente do desempenho da equipe, detalhando métricas de desempenho geral e médio para cada equipe dentro de uma temporada competitiva específica

<b>player.csv</b> - Análise agregada de desempenho dos jogadores, apresentando métricas abrangentes de desempenho individual e médio dos jogadores ao longo de uma temporada competitiva.

<b>hero.csv</b> - Estatísticas de seleção, banimento e vitória de campeões (heróis) em uma temporada competitiva, oferecendo insights sobre o meta e a eficácia dos campeões.

<b>team_vs.csv</b> - Análise de desempenho interpessoal da equipe, documentando confrontos diretos e desempenho comparativo da equipe dentro de uma temporada competitiva.

<b>player_vs.csv</b> - Comparação de desempenho individual de jogadores, rastreando confrontos entre jogadores e métricas de desempenho individual ao longo de uma temporada competitiva.

<b>hero_vs.csv</b> - Análise de desempenho de confrontos de campeões, fornecendo insights detalhados sobre o desempenho de diferentes campeões entre si em partidas competitivas.

<b>hero_chosen.csv</b> - Preferências históricas de seleção de campeões, revelando as escolhas de campeões e estratégias dos jogadores ao longo da temporada competitiva.

<hr>
<br>

<h1>Documentação mais Detalhada em Vídeo</h1>

<h2>Processo de ETL</h2>
<h4><a href="https://www.youtube.com/watch?v=AphyvqN_cC0&list=PL32Jw9MJZGxU7ZPl_HRPCE8jHXt1KDL5g&index=2&ab_channel=MateusFran%C3%A7a-AnalistadeBi"> <b>Acesse aqui</b> </a></h4>

<br>

<h2>Processo de Criação do Dashboard</h2>
<h4><a href="https://www.youtube.com/watch?v=F023oyW_W5I&list=PL32Jw9MJZGxU7ZPl_HRPCE8jHXt1KDL5g&index=2&ab_channel=MateusFran%C3%A7a-AnalistadeBi"> <b>Acesse aqui</b></a></h4>

<hr>
<br>

<h1>Documentação Escrita</h1>

<h2>1. Resumo do Projeto</h2>

<br>

<h3><b>Competitivo League of Legends</b></h3>

<br>

<h3><b>Objetivo:</b></h3> 
Com o aumento das apostas esportivas no cenário de E-sports (Esportes Eletrônicos) e comigo já fazendo parte desse mundo de apostas há algum tempo, me vi na responsabilidade de criar um Dashboard Analítico para me auxiliar e também auxiliar diversos apostadores a tomar decisões fundadas e baseadas em dados reais e verídicos, aumentando assim a chance de sucesso nas apostas no cenário competitivo do jogo League of Legends.

<br>

<h3><b>Fonte dos Dados:</b></h3>
Data Warehouse, Arquivo Delimitado por Vírgula, arquivos CSV

<br>

<h3><b>Ferramentas Utilizadas:</b></h3> 
Power BI, SQL Server Management Studio 20, Visual Studio 2022 (SSIS)

<hr>
<br>

<h2>2. Coleta e Preparação dos Dados</h2>

<h2><b>Descrição da Base</b></h2>

<br>

<h3><b>Quantidade de registros:</b></h3>
1.206.725 Registros

<br>

<h3><b>Principais colunas:</b></h3> 
MatchID, matchType, conjunto de jogos, MatchDate, Duração, vitória, TeamN, região, Barão, Dra, Torres destruídas, {Team}_banN, {Team}_playerN_{Atributos}, {Team}_{Player}_name,{Equipe}_{Jogador}_escolha.

<br>

<h3><b>Tratamento de Dados:</b></h3>
Toda a parte de ETL foi feita no Visual Studio (SSIS), e depois carregado em um Data Warehouse criado.
Remoção de Nulos, vazios, unpivot de colunas, normalização dos dados, alteração de tipos de dados, extração de caracteres, mudança na regição padrão de data.

<br>
<hr>

<h2>3. Análise Exploratória</h2>

<h3><b>Principais Estatísticas:</b></h3>
Médias, medianas, distribuições, correlações

<br>

<h3><b>Visualizações:</b></h3>
Cartão, Gráfico de barras clusterizado, Gráfico de linhas, Segmentador de dados, Gráfico de área empilhado, Gráfico de colunas empilhadas, Gráfico de área, Gráfico de colunas clusterizado, Matriz e Gráfico de barras empilhadas.

<br>

<h3><b>Tendências e Padrões:</b></h3>
Banimentos de campeões por times, Quantidade de Dragões, Barões e torres por times, podendo filtrar e fazer uma comparação entre dois times.
Campeões mais jogados e mais vitoriosos.
Jogadores mais vitoriosos, que deram mais danos, que obtiveram mais abates e assistências.
Times mais vitoriosos, que fazem mais objetivos.

<hr>
<br>

<h2>4. Modelagem e KPIs</h2>

<h3><b>Dashboards e Relatórios:</b></h3>
<br>
<b>Dashboard de Jogos:</b> Exibe o resumo geral com os principais indicadores sobre os jogos disputados de todos os campeonatos, podendo filtrar por times.
<b>Dashboard de Campeões:</b> Exibe o resumo geral da performance de campeões por times, jogadores e jogos disputados.
<b>Dashboard de Campeões VS:</b> Exibe os detalhes de Campeões vs Campeões.
<b>Dashboard de Players:</b> Exibe o resumo geral da performance de jogadores.
<b>Dashboard de Players VS:</b> Exibe os detalhes comparando jogador vs jogador.
<b>Dashboard de Time:</b> Exibe o resumo geral dos times com os principais indicadores.

<br>

<h3><b>Insights Gerados:</b></h3>
Aumento de 25% no acerto de apostas esportivas no cenário competitivo de League of Legends.

<hr>
<br>

<h2>5. Conclusão e Próximos Passos</h2>

<h3><b>Resumo dos Principais Resultados:</b></h3>
Aprendi bastante sobre modelagem de dados e criação de Data Warehouse, principalmente sobre o processo de ETL e normalização dos dados.

<br>

<h3><b>Limitações do Projeto:</h3></b>
Base de dados sem documentação, tive que passar um dia inteiro apenas documentando e estudando os dados que iria usar.
Dados totalmente desnormalizados, todos os dados em um arquivo simples, altamente bagunçado e totalmente desestruturado.

<br>
  
<h3><b></b>Sugestões para Melhorias Futuras:</h3></b>
Trazer insights futuros sobre as organizações (Times) incluindo staffs, coaches, etc.
Melhorar alguns gráficos, e trazer opções de mais filtros.
Trazer um novo Dashboard para analisar os campeonatos sendo filtrados por regiões.

<br>
<hr>

