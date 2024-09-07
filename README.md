# Bitcoin-return-forecast
Prévision de rendement sur un carnet d'ordre de cryptomonnaie : cas du bitcoin

Le challenge de notre projet de machine learning consiste à prédire les rendements sur des cryptomonnaies (bitcoin) en se basant sur le carnet d'ordre et les trades passés.

Nous avons téléchargé deux fichier csv, un avec le carnet d'ordre actuel (du jour de téléchargement - 21 avril 2024), et le second avec les trades passés, soit les ordres exécutés.

Pour répondre à ce sujet, nous allons suivre une approche en plusieurs étapes :

1) preprocessing avec export et formatage des données : nous commencerons par extraire les données pertinentes (carnet d'ordre et trades passés) et les formater de manière appropriée pour les utiliser dans notre modèle :

1.1) statistique descriptives

1.2) graphs

2) recherche de notre variable target : rendements

3) recherche de features pertinentes : nous explorerons différentes variables explicatives ou caractéristiques du marché pour identifier celles qui ont le plus d'influence sur les rendements du carnet d'ordres.

4) construction des modèles : nous allons développer trois types de modèles :

4.1) modèle simple : un modèle de référence pour évaluer la performance de nos autres modèles (type MCO)

4.2) modèle non supervisé (moins pertinent pour notre problématique, nous avons un problème de regression) : nous explorerons également des approches non supervisées pour en extraire éventuellement des informations utiles via le modèle PCA.

4.3) modèle supervisé : coeur de notre approche, nous entraînerons des modèles supervisés pour prédire les rendements du carnet d'ordres en fonction de nos différentes features.

5) Analyse des résultats et comparaison des différents modèles

6) Conclusion

Pour information, le projet initial était sur la crypto bal, qui est moins liquide, mais les résultats étaient que très peu cohérents car les relations entre nos features et notre variable cible étaient très bruités. Nous avons donc choisi de nous tourner vers une cryptomonnaie beaucoup plus liquide, comme le bitcoin qui met en évidence des relations plus évidentes. (nous avons quand meme inséré les deux csv sur la crypto bal, via bal.csv et bal-trades.csv ).

Ce projet peut donc être adapté a la cryptomonnaie de votre choix.
