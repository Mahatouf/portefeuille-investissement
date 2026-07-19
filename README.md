# Évaluation de la performance d'un portefeuille d'investissement

## Contexte
Analyse quantitative d'un portefeuille composé d'actions et d'ETF, pour en évaluer le risque et la performance ajustée au risque.

## Objectif
Fournir des indicateurs financiers clés (rendement, volatilité, ratio de Sharpe) permettant de comparer plusieurs stratégies d'allocation.

## Données
- Source : Yahoo Finance (librairie `yfinance`)
- Actifs : à préciser selon le portefeuille choisi (ex : 5-10 actions/ETF)
- Période : 5 dernières années (cours de clôture ajustés, quotidiens)

## Méthodologie
1. Récupération des cours historiques via `yfinance`
2. Calcul des rendements journaliers et annualisés
3. Calcul de la volatilité (écart-type annualisé)
4. Calcul du ratio de Sharpe (rendement excédentaire / volatilité)
5. Visualisation : courbe de performance cumulée, drawdown, corrélations entre actifs

## Outils
Python — pandas, numpy, matplotlib/seaborn, yfinance

## Résultat
- Notebook Jupyter documenté : `analyse_portefeuille.ipynb`
- Lien vers le dashboard/rapport : *(lien à ajouter)*

## Comment reproduire
```bash
pip install -r requirements.txt
jupyter notebook analyse_portefeuille.ipynb
```

## Limites
Analyse à but démonstratif — ne constitue pas un conseil en investissement.

## Auteur
Mahatouf ALASSANI — Data Analyst & Économiste en finances internationales
[mahatoufalassani@gmail.com](mailto:mahatoufalassani@gmail.com) · [LinkedIn](https://www.linkedin.com/in/mahatouf-alassani)

