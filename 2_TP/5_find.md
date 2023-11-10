
*Pour lire cette partie du TP, tu dois :*
- *Avoir lancé le script `./start.sh`

---
---

Oh, là, là misère !! C'était un piège !
Apparemment un virus avec un compte à rebours s'est déclenché ?!

**Bon, leçon numéro 1 : on vérifie toujours ce qu'on exécute !!**

Il y a un nouveau fichier : `sortie.log`.
Affiche son contenu avec la commande `cat`.

Il reste un peu moins de 2h donc pour trouver comment arrêter ce processus...
Mais il faudra déjà savoir quel nom ce processus porte !
Tu peux utiliser la commande `htop` pour voir tous les processus... peut-être qu'un nom de processus te sautera aux yeux, comme *virus* ?

> Parcours les processus affichés avec `htop` pour voir si un processus apparait comme suspect.

---

<details>
  <summary>Rien ne me saute aux yeux</summary>

Peut-être que l'auteur de ce script a laissé des traces pour retrouver le nom de ce processus ... en faisant des tests, il a peut-être laissé une porte de secours !
Utilises la commande `find` pour chercher dans un répertoire donné, un fichier qui porte un nom que tu lui donnes en paramètre. Tu peux essayer de chercher des mots-clé comme :
- virus
- stop
- defuse
- backdoor
- help
- ...

Il est peu probable que le fichier s'appelle uniquement `virus` par exemple, mais il peut contenir un mot-clé. Donnes la correct instruction à `find` pour chercher si un mot-clé est contenu dans le nom du fichier.
</details>


---
---
*A la fin de cette partie, tu devrais maitriser comment :*
- *Visualiser le contenu d'un fichier avec `cat`*
- *Voir la liste de tous les processus avec `htop`*
- *Rechercher un fichier qui porte un nom spécifique avec la commande `find`*
