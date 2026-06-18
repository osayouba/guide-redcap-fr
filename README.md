# REDCap Guide FR

> Documentation collaborative REDCap en français, à destination des administrateurs, data managers, ARC et biostatisticiens travaillant en recherche clinique.

[![GitLab Pages](https://img.shields.io/badge/Site-GitLab%20Pages-orange)](https://votre-groupe.gitlab.institutionnel.org/redcap-guide-fr)
[![Quarto](https://img.shields.io/badge/Built%20with-Quarto-blue)](https://quarto.org/)
[![Licence](https://img.shields.io/badge/Licence-CC%20BY%204.0-green)](LICENSE)

---

## Structure du projet

```
redcap-guide-fr/
├── _quarto.yml                  # Configuration du livre Quarto
├── index.qmd                    # Page d'accueil
├── resources/
│   └── custom.scss              # Thème CSS personnalisé
├── fiches/
│   ├── admin/                   # Fiches administrateur REDCap
│   ├── data-manager/            # Fiches data manager / ARC
│   ├── api-r/                   # Fiches API et intégration R
│   └── investigateur/           # Fiches à destination des investigateurs
└── .gitlab-ci.yml               # Pipeline CI/CD → GitLab Pages
```

## Prérequis locaux

Pour compiler le site en local, vous avez besoin de :

- [Quarto ≥ 1.5](https://quarto.org/docs/get-started/)
- R ≥ 4.3 avec les packages : `rmarkdown`, `knitr`, `REDCapR`, `dplyr`, `ggplot2`

```bash
# Compiler et prévisualiser en local
quarto preview

# Compiler sans prévisualisation
quarto render
```

## Contribuer

Les contributions sont encouragées ! Pour proposer une modification :

1. Forker le dépôt ou créer une branche depuis `main`
2. Modifier ou créer un fichier `.qmd` dans le dossier `fiches/` approprié
3. Vérifier le rendu en local avec `quarto preview`
4. Soumettre une **Merge Request** vers `main`

### Ajouter une nouvelle fiche

1. Créer le fichier `.qmd` dans le bon sous-dossier
2. L'ajouter dans `_quarto.yml` sous la section `chapters:` correspondante
3. Suivre la structure des fiches existantes (présentation, exemples, points d'attention, références)

## Licence

Ce contenu est distribué sous licence **Creative Commons Attribution 4.0 International (CC BY 4.0)**.  
Vous pouvez librement partager et adapter ce contenu, à condition de citer la source.

---

*Inspiré du projet [utilitR](https://book.utilitr.org/) de l'INSEE.*
