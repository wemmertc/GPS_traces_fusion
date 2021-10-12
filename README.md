# GPS traces fusion
> Hackathon TPS 2021

## Objectifs
1. trouver l'ensemble des points d'intersection à partir des traces brutes
2. générer les segments reliant ces points d'intersection

dans le répertoire data :
- `blaesheim.geojson` : ensemble des traces brutes à fusionner
- `blaesheim_gt.geojson` : vérité terrain contenant les croisements et les segments réels à trouver
- `blaesheim_result_example.geojson` : exemple de fichier résultat à générer pour utiliser la fonction d'évaluation
