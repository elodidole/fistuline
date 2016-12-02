fistuline
=========


### les outils

- github desktop (synchronisation)
- atom (édition)
- Terminal (preview)


### preview

#### étape 1

Pour pouvoir prévisualiser le site, tout d'abord ouvrir l'application ```Applications/Utilities/Terminal``` puis écrire dans la fenêtre du terminal.

```
source venv/bin/activate
cd Documents/travail\ en\ cours
```

#### étape 2

Régénérer le site avant chaque preview avec la commande
```
sectioner build fistuline/source fistu-web
```


Le site est bon pour previsualisation dans le dossier ```Documents/travail en cours/fistu-web```

#### étape 3

Réitérer l'étape 1 de telle manière à disposer d'une deuxième fenêtre de terminal dans laquelle il faut écrire

```
cd fistu-web && python -m http.server 8000
```

le site est maintenant visible a l'adresse [http://localhost:8000](http://localhost:8000)

### ajouter des pages
créer un nouveau fichier xml dans le dossier fistuline/source/pages sur atom
J'utilise la page vide dans les pages je la complète et puis je référence son nom dans les datas en créant un nouveau, je le met ou je veux dans l'ordre.
