# GPS traces fusion
> Hackathon TPS 2021

## Contexte
Dans le cadre de la cartographie, beaucoup d'investissements sont faits pour avoir des cartes routières à jour et permettre aux utilisateurs de s'orienter efficacement. Cependant, dans le cadre de la randonnée, la mise à jour des cartes reste très coûteuse en temps et ne peut être faite régulièrement. Par exemple, une carte de randonnée Top 25 de l'IGN n'est actualisée que tous les 6 à 10 ans !
Cependant, la collecte de données utilisateur a considérablement augmenté depuis la démocratisation des smartphones, il y a une dizaine d’années. Ces données sont potentiellement une source considérable d’informations utilisables à des fins diverses. Une application extrêmement utile serait de pouvoir construire, mettre à jour et rendre exploitable une base de données des sentiers existants à partir de traces GPS acquises par des utilisateurs lors de leurs déplacements.

C'est ce challenge que nous vous demandons de relever aujourd'hui !


## Objectifs
1. trouver l'ensemble des points d'intersection à partir des traces brutes
2. générer les segments reliant ces points d'intersection

dans le répertoire data :
- `blaesheim.geojson` : ensemble des traces brutes à fusionner
- `blaesheim_gt.geojson` : vérité terrain contenant les croisements et les segments réels à trouver
- `blaesheim_result_example.geojson` : exemple de fichier résultat à générer pour utiliser la fonction d'évaluation
