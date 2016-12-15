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
pour naviguer plus facilement d'une appli à l'autre cmd tab
créer un nouveau fichier xml dans le dossier fistuline/source/pages sur atom
J'utilise la page vide dans les pages je la complète et puis je référence son nom dans les datas en créant un nouveau, je le met ou je veux dans l'ordre.
### Pour enlever des pages
je vais dans data, je les sélectionne et je fais shift/cmd/slash, ça les met en attente (non actives) je peux les remettre après en refaisant la même chose
Pour chercher un éléments dans toutes les pages shift/cmd/F (find)


Si je fais des sous dossiers pour classer mes fichiers images j'essaye que ça soit cohérent avec mes pages et je dois changer le nom dans atom sur mes pages en ajoutant le nom du sous dossier <gallery root="images/ici">

Quand j'ai fini un boulot, je fais commit sur github après avoir mis dans les commentaires une descritpion de ce que j'ai fait et je synchronise

faire un petit fichier png ou svg pour les boutons rouges et bleu
dans templates master je dois changer les infos pour y mettre les miennes
