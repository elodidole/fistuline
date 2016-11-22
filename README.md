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
