# Classement mondial de la criminalité

Ce projet contient un tableau au format Markdown présentant le classement mondial des pays selon leur indice de criminalité et de sécurité.

## Contenu

- `classement_criminalite.md` : Tableau complet des 147 pays classés par indice de criminalité (du plus élevé au plus faible) avec leur indice de sécurité correspondant.
- `criminalite_securite.csv` : Données au format CSV du classement des pays par indice de criminalité et de sécurité.
- `pib_par_habitant.csv` : Données au format CSV du classement des pays par PIB par habitant selon les données du FMI de 2017.
- `gini.csv` : Données au format CSV des indices de Gini (inégalité des revenus) par pays.
- `iojp.csv` : Données au format CSV de l'Indice d'Oppression Judiciaire et Policière (IOJP) par pays.
- `index.html` : Application web interactive affichant un graphique de la relation entre le PIB par habitant et l'indice de criminalité.
- `gini_criminalite.html` : Application web interactive affichant un graphique de la relation entre l'indice de Gini et l'indice de criminalité.
- `iojp.html` : Application web interactive affichant un graphique et un tableau des scores de l'Indice d'Oppression Judiciaire et Policière par pays.
- `iojp_criminalite.html` : Application web interactive affichant un graphique de la relation entre l'Indice d'Oppression Judiciaire et Policière et l'indice de criminalité.
- `pib_iojp.html` : Application web interactive affichant un graphique de la relation entre le PIB par habitant et l'Indice d'Oppression Judiciaire et Policière.
- `densite_criminalite.html` : Application web interactive affichant un graphique de la relation entre la densité de population et l'indice de criminalité.

## Utilisation

Vous pouvez visualiser le tableau directement dans GitHub ou tout autre éditeur compatible avec Markdown.

Pour visualiser les graphiques interactifs, lancez un serveur web local dans le répertoire du projet :

```bash
python -m http.server 8000
```

Puis ouvrez votre navigateur à l'adresse : http://localhost:8000

L'application propose six visualisations différentes :
- PIB par habitant vs Indice de criminalité : http://localhost:8000/index.html
- Indice de Gini vs Indice de criminalité : http://localhost:8000/gini_criminalite.html
- Indice d'Oppression Judiciaire et Policière (IOJP) : http://localhost:8000/iojp.html
- IOJP vs Indice de criminalité : http://localhost:8000/iojp_criminalite.html
- PIB par habitant vs IOJP : http://localhost:8000/pib_iojp.html
- Densité de population vs Indice de criminalité : http://localhost:8000/densite_criminalite.html

## Visualisations disponibles

1. **PIB vs Criminalité** (index.html) : Graphique interactif montrant la relation entre le PIB par habitant et l'indice de criminalité.
2. **Gini vs Criminalité** (gini_criminalite.html) : Graphique interactif montrant la relation entre le coefficient de Gini (inégalités) et l'indice de criminalité.
3. **IOJP** (iojp.html) : Visualisation de l'Indice d'Oppression Judiciaire et Policière (IOJP) par pays.
4. **IOJP vs Criminalité** (iojp_criminalite.html) : Graphique interactif montrant la relation entre l'IOJP et l'indice de criminalité.
5. **PIB vs IOJP** (pib_iojp.html) : Graphique interactif montrant la relation entre le PIB par habitant et l'IOJP.
6. **Densité vs Criminalité** (densite_criminalite.html) : Graphique interactif montrant la relation entre la densité de population et l'indice de criminalité.

## Fonctionnalités

- Visualisation interactive des données
- Possibilité de basculer entre échelle linéaire et logarithmique pour le PIB
- Affichage des lignes de régression
- Filtrage des valeurs extrêmes
- Affichage des étiquettes des pays
- Informations détaillées sur chaque pays au survol ou au clic

## Observations

- Les pays ayant les indices de criminalité les plus élevés sont le Venezuela (80,70), la Papouasie-Nouvelle-Guinée (80,30) et Haïti (78,87).
- Les pays les plus sûrs sont Andorre (15,29), les Émirats Arabes Unis (15,49) et le Qatar (15,79).
- L'indice de sécurité est complémentaire à l'indice de criminalité (leur somme est égale à 100).
