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

Essaq tabela exibe dados das equipes.

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
