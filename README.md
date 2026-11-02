# Bilan carbone 2024 du laboratoire ESYCOM

Bilan des émissions de gaz à effet de serre (scopes 1 à 3) du laboratoire **ESYCOM** (CNRS, UMR 9007) pour l'année 2024, accompagné d'une application web de calcul et de projection des émissions.

Projet académique réalisé en équipe à ESIEE Paris (2025 – 2026).

**Site en ligne : https://alessandro-digalloclauss.github.io/bilan-carbone-ESYCOM/**

## Objectif

- Quantifier l'empreinte carbone 2024 du laboratoire, poste par poste : achats, missions, énergie des bâtiments, construction, trajets domicile-travail, matériel informatique.
- Identifier les postes prioritaires et simuler des leviers de réduction au regard de la trajectoire CNRS 2030 (−50 %).

Résultat : **385,5 tCO₂eq**, soit **7,49 tCO₂eq par ETP** (51,5 ETP). Les achats représentent 61 % du total, les missions 22 %.

## Contenu de l'application

- Saisie ou import CSV des données d'activité par poste
- Calcul des émissions et graphiques de répartition
- Évolution 2022 – 2024 et scénarios de projection
- Combinaison de mesures de réduction et indicateurs normalisés (format GES-1point5)

## Technologies

HTML, CSS et JavaScript sans framework, graphiques [Chart.js](https://www.chartjs.org/), données en CSV. Méthodologie et facteurs d'émission : outil GES-1point5 (Labos 1point5) et Base Carbone de l'ADEME.

## Structure

| Fichier / dossier | Rôle |
|---|---|
| `bilan_carbone_esycom2024_multilabos_v4.html` | Application web (calculs, graphiques, scénarios) |
| `index.html` | Page d'accueil GitHub Pages, redirige vers l'application |
| `données_esycom.md` | Données sources : surfaces, énergie, enquêtes |
| `import_GES1point5/` | Données converties au format d'import GES-1point5 |
| `resutat labo 1poin5/` | Résultats exportés depuis GES-1point5 |
| `*.xlsx` | Extractions brutes (achats, missions, commandes) |

## Lancer le projet

Aucune installation : ouvrir `bilan_carbone_esycom2024_multilabos_v4.html` dans un navigateur, ou consulter le site en ligne ci-dessus.

```bash
git clone https://github.com/alessandro-digalloclauss/bilan-carbone-ESYCOM.git
cd bilan-carbone-ESYCOM
open bilan_carbone_esycom2024_multilabos_v4.html
```
