# Firmwares TBRT publiés

Les firmwares que les outils TBRT proposent d'eux-mêmes aux boîtiers des
clients. Aujourd'hui : **AUX-N**, mis à jour par la page AUX-N manager.

**Déposer un fichier ici, c'est le LIVRER** : chaque client qui connecte un
boîtier plus ancien se verra proposer cette version. N'y déposer qu'une
version validée.

## Déposer une version

1. Ouvrir le dossier du produit (`aux-n/`), puis **Add file → Upload files**.
2. Glisser le `.hex`, nommé **`aux-n-<version>.hex`**, par exemple
   `aux-n-26.10.64.49.hex` : la version est celle qu'affiche la console.
3. **Commit changes**.

La page propose la version **la plus haute** du dossier. Elle vérifie,
avant d'écrire quoi que ce soit, que le fichier est arrivé entier, que c'est
un firmware AUX-N et que la version gravée dedans est celle du nom : un
fichier mal nommé est refusé.

Retirer une version : supprimer son fichier. La précédente redevient la
plus haute — mais un boîtier qui a déjà la version retirée la garde (la
page ne propose jamais de redescendre).

## Pourquoi un dépôt public, à part

Les sources sont dans le dépôt privé `tbrt`. Une page web ne peut lire
qu'un dépôt public, et GitHub autorise la lecture de ses fichiers par un
autre site (les « Releases », non). Les `.hex` sont donc publics : sans le
boîtier ils ne servent à rien.
