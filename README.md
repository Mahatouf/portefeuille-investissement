# Évaluation de la performance d'un portefeuille d'investissement

**[Voir le dashboard en direct →](https://mahatouf.github.io/portefeuille-investissement/)**

## Contexte
Analyse quantitative d'un portefeuille composé de 6 actifs (actions et ETF), pour en évaluer le risque et la performance ajustée au risque sur 5 ans.

## Objectif
Fournir des indicateurs financiers clés (rendement, volatilité, ratio de Sharpe, drawdown, corrélations) permettant de comparer la performance de chaque actif et la solidité du portefeuille dans son ensemble.

## Données
- Source : Yahoo Finance (via la librairie `yfinance`)
- Actifs : Apple (AAPL), Microsoft (MSFT), Alphabet (GOOGL), LVMH (MC.PA), ETF S&P 500 (SPY), ETF Obligations US (AGG)
- Période : juillet 2019 – juillet 2024 (cours de clôture quotidiens, 1248 jours de bourse)

## Méthodologie
1. Récupération des cours historiques via l'API `yfinance`
2. Calcul des rendements journaliers, puis annualisés
3. Calcul de la volatilité (écart-type annualisé)
4. Calcul du ratio de Sharpe (taux sans risque : 2 %)
5. Calcul du drawdown du portefeuille équipondéré (perte depuis le dernier sommet)
6. Matrice de corrélation entre tous les actifs

## Résultats clés
- **Apple** affiche le meilleur ratio de Sharpe (**1,02**) sur la période, avec un rendement annualisé de 34,8 %
- Le portefeuille équipondéré affiche un rendement annualisé de **21,5 %**, une volatilité de **20,2 %** et un ratio de Sharpe de **0,96**
- Le drawdown maximum du portefeuille a atteint **-25,2 %** (marché baissier de 2022)
- L'**ETF Obligations US (AGG)**, malgré un rendement quasi nul (-0,05 %), présente une corrélation moyenne de seulement **0,15** avec les autres actifs — un vrai amortisseur de risque en période de baisse des marchés actions

## Outils
Python — pandas, numpy, yfinance ; dashboard HTML/JavaScript (Chart.js)

## Comment reproduire
1. Cloner ce repo
2. Ouvrir `index.html` dans un navigateur — aucune dépendance à installer

## Limites
Analyse à but démonstratif — ne constitue pas un conseil en investissement.

## Auteur
Mahatouf ALASSANI — Data Analyst & Économiste en finances internationales
[mahatoufalassani@gmail.com](mailto:mahatoufalassani@gmail.com) · [LinkedIn](https://www.linkedin.com/in/mahatouf-alassani) · [Portfolio](https://mahatouf.github.io/portfolio/)

