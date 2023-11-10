_Pour lire cette partie du TP, tu dois :_

- _Avoir copié le contenu de `pit.iso` dans un dossier sous `/home/user`_

---

---

Explorons cet iso désormais !

Tu peux réaliser un `ls` pour voir tous les fichiers contenus :

```
user@DEBIAN:~/Downloads/ISO$ ls
OS.iso  processName  start.sh
```

Mmh, ça ne ressemble pas vraiment à ce quoi je m'attendais. Il y a l'air d'avoir un script bash : `start.sh`. Essaies de le lancer, ça lancera peut-être le film directement ?

Avant de lancer un script, il faut que le fichier ait la permission de pouvoir s'exécuter !
Pour éditer le permission, utilses la commande `chmod` sur le fichier souhaité :

- avec l'option `+` pour ajouter des droits
- avec l'option `-` pour supprimer des droits
- `r` : droits de lecture
- `w` : droits d'écriture
- `x` : droits d'exécution

Donne (au minimum) les droits nécessaire à l'exécution du script, puis lance le script ! On verra ce qu'il se passe ...

---
---

_A la fin de cette partie, tu devrais maitriser :_

- _La visualisation du système de fichiers avec `ls`_
- _Lancer un script `bash`_
- _Editer les drotis d'exécution d'un fichier avec `chmod`_
