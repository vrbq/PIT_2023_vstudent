_Pour lire cette partie du TP, tu dois :_

- _Avoir téléchargé le fichier `pit.iso`_

---

---

Maintenant que tu as téléchargé l'iso, il faut **monter** ce fichier.

> _Qu'est-ce qu'un fichier iso ?_

Les fichiers _.iso_ sont souvent apparentés à des disques. On imagine ici par exemple que le publicitaire à graver le film du client sur un DVD, puis à réalisé une copie complète du DVD sous format .iso.

Cela peut servir par exemple à inclure toutes les subtilités, comme le menu ou le choix des sous-titres. Bon, c'est un peu bizarre comme choix pour transmettre un film mais passons !

1. Tout d'abord, créer un nouveau dossier `mount_point` dans le dossier `/mnt`, avec la commande `mkdir`.
2. Monte le fichier .iso grâce à la commande `mount`.
   1. Tu auras besoin de renseigner l'emplacement de ton fichier.iso mais aussi l'endroit où tu veux le monter (ici, dans `mount_point`).
   2. L'option `loop` te sera nécessaire aussi !
   3. Tu devras aussi lancer cette commande via le super utilisateur, en mettant `sudo` devant ta commande. Je t'en reparle plus tard.
3. Une fois l'iso montée, tu pourras te rendre dans le dossier `mount_point` avec la commande `cd`.
4. Copies alors tout le dossier `mount_point` vers un dossier que tu maitrises plus (par exemple, `Downloads`, `Desktop` ou n'importe quel autre dossier présent dans ton dossier utilisateur `home/user`).
   1. Tu auras certainement besoin de l'option `-r` qui permet de copier _récursivement_ tous les sous-dossiers du dossier que tu souhaites copier.
5. Tu peux alors te rendre dans ce dossier pour vérifier que la copie s'est effectuée sans soucis.

---

---

_A la fin de cette partie, tu devrais maitriser :_

- _La création de dossier avec `mkdir`_
- _Le montage de fichier iso avec `mount`_
- _La navigation dans le système de fichier avec `cd`_
- _La copie d'un dossier entier avec `cp`_
