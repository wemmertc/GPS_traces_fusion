# GPS traces fusion
> Hackathon TPS 2021

## Contexte
Dans le cadre de la cartographie, beaucoup d'investissements sont faits pour avoir des cartes routières à jour et permettre aux utilisateurs de s'orienter efficacement. Cependant, dans le cadre de la randonnée, la mise à jour des cartes reste très coûteuse en temps et ne peut être faite régulièrement. Par exemple, une carte de randonnée Top 25 de l'IGN n'est actualisée que tous les 6 à 10 ans !
Cependant, la collecte de données utilisateur a considérablement augmenté depuis la démocratisation des smartphones, il y a une dizaine d’années. Ces données sont potentiellement une source considérable d’informations utilisables à des fins diverses. Une application extrêmement utile serait de pouvoir construire, mettre à jour et rendre exploitable une base de données des sentiers existants à partir de traces GPS acquises par des utilisateurs lors de leurs déplacements.

C'est ce challenge que nous vous demandons de relever aujourd'hui !


## Objectifs
Il y a deux objectifs dans ce challenge :
1. trouver l'ensemble des points d'intersection à partir de traces GPS brutes ;
2. générer les segments reliant ces points d'intersection.

Pour cela, vous disposerez de deux jeux de données distincts. Le premier, appelé `blaesheim.geojson` correspond  à un jeu de 39 traces acquises sur la commune de Blaesheim avec une montre GPS très précise. Ce jeu de données est très propre et va permettre à servir de benchmarkl à votre méthode. 
La vérité terrain (listes des intersections à trouver et des segments) est contenue dans le fichier `blaesheim_gt.geojson`.
Enfin le fichier `blaesheim_result_example.geojson` représente un exemple de fichier résultat à générer pour utiliser la fonction d'évaluation ().
Le second jeu de données, `blaesheim_visorando.geojson` correspond à des traces extraites de la base de données de l'application Visorando. Les données sont nettement moins propres :-(
Vous pourrez l'utiliser une fois que vous aurez quelque chose de fonctionnel pour vous rendre compte que le problème est difficile !

## Manipulation des fichiers .geojson
Pour visualiser le contenu des fichiers `.geojson` vous pouvez utiliser le site [geojson.io](geojson.io). Il suffit de faire un glisser-déposer des fichiers sur la carte pour les visualiser.
Pour manipuler les fichier en python, vous pouvez utiliser la librairie [geojson](https://pypi.org/project/geojson/)
