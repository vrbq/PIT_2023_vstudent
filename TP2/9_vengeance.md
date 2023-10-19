
*Pour lire cette partie du TP, tu dois :*
- *Avoir supprimer l'utilisateur `hacker` qui a été créé par l'auteur du virus*
---
---

Bon désormais, on va essayer de retrouver ce malandrin ! Essaies de chercher des traces de son passage dans tout ce que tu as...

> Cherches des traces avant de lire la suite !

---

<details>
  <summary>J'ai trouvé des traces !</summary>


...comme par exemple un fichier qui s'appellerait `OS.iso` ? Ce qui serait fou, c'est que ça soit une copie de l'OS de l'auteur du virus...

Il faudrait que tu `umount` l'iso qui est actuellement montée, et que tu `mount` celle-ci pour voir s'il y a quelque chose d'intéressant.

</details>

---

> Ca devient de plus en plus intéressant !
> On dirait que tu as désormais accès à des restes de dossiers appartenant à l'OS de l'auteur du virus.
> Fouilles un peu, notamment si un nom d'utilisateur ressort


<details>
  <summary>Un nom d'utilisateur ? </summary>

Il faut de nouveau chercher dans `/etc/passwd` pour voir un nom d'utilisateur un peu particulier apparaître ...

</details>

> Maintenant que tu as un nom d'utilisateur, il faudrait pouvoir le lier à quelque chose de plus concret !
> Et si on jetait un coup d'oeil dans le dossier `Logs` ?

<details>
  <summary> Il y a beaucoup d'informations dans ces fichiers ... </summary>

Dans le dossier `Logs` se trouve de nombreux fichiers. Mais comment savoir lequel pourrait nous être utile ?

Pour faire apparaitre une partie du fichier - afin de te donner une idée du contenu - tu peux utiliser les commandes :
- `tail` : qui fait apparaitre la fin d'un fichier
- `head` : qui en fait apparaitre le début

</details>

<details>
  <summary> Un fichier qui attire l'oeil </summary>

Tous les fichiers finissent en `.log` sauf un... à quoi pourrait correspondre l'extension `.nc` ?

Et si tu essaies de l'ouvrir avec `cat`, on va peut-être trouver des infos qui croustillent ?

Fais des recherches pour t'aiguiller

</details>




---
---
*A la fin de cette partie, tu devrais maitriser comment :*
- *Dé-monter un fichier monté avec `unmount`*
- *Voir le début et la fin d'un fichier avec `head` et `tail`*
- *Comprendre à quoi correspond une extension inconnue*
