# demo-seeds

Données de démonstration générées (fixtures Django + images libres de droit) pour les
projets basés sur [`django-react-starter`](https://github.com/philbotche/django-react-starter).

Ce dépôt est public : il ne contient que des données synthétiques (noms, textes générés)
et des images libres de droit ([Picsum](https://picsum.photos)), jamais de données réelles.

## Structure

```
<slug-du-projet>/
  <app_label>/
    fixtures.json   # export Django (dumpdata) de l'app
    media/          # fichiers médias référencés par la fixture, arborescence identique à MEDIA_ROOT
```

## Utilisation

Voir la section « Seed de démonstration » du `CLAUDE.md` du starter :

- `generate_demo_seed --count N` (dans le projet dérivé) génère le contenu d'un dossier
  `<app_label>/` ci-dessus, en local (`backend/seed_data/<app_label>/`).
- Publication manuelle ici, sous `<slug-du-projet>/<app_label>/`.
- `install_demo_seed <app_label>` (dans le projet dérivé) télécharge ce dépôt et installe
  le sous-dossier correspondant.
