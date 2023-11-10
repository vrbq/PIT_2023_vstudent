_Pour lire cette partie du TP, tu dois :_

- _Avoir trouver l'intérêt du fichier `trafic.log.nc`_

---

---

<details>
  <summary> Un fichier qu'on ne peut pas ouvrir </summary>

Quand on essaies d'ouvrir ce fichier, on n'y comprends rien !

Alors, ce fichier est crypté !

Mais avec quel utilitaire ce fichier a-t-il été encodé ? Peut-être qu'on trouvera avec quelques recherches sur l'extension `.nc` et son cryptage ... ou quelques recherches dans le dossier `Logs` si un autre indice a été laissé ?

</details>

<details>
  <summary> J'ai trouvé le nom de l'utilitaire</summary>

Bingo ! Heuresement que ce "hacker" est vraiment pas fut-fut et qu'il a mis le nom de cet utilitaire dans un fichier en clair !

Mais est-ce qu'on possède cet utilitaire ?

Pour savoir, tu peux utiliser la commande `dpkg -l` qui dresse la liste de tous les utilitaires installés sur le poste.
Tu peux soit parcourir un a un les noms pour vérifier ou alors, de nouveau utiliser `grep`.

</details>

<details>
  <summary>L'utilitaire n'est pas dans la liste...</summary>

Ne t'en fais pas, parce que s'il n'est pas dans la liste des programmes, ça veut dire qu'on doit l'installer !

Pour installer un paquet, il faut utiliser la commande :
`sudo apt-get install <nom_du_paquet>`

C'est parti, installe cet outil de cryptage !

</details>

---

---

_A la fin de cette partie, tu devrais maitriser comment :_

- _Dresser la liste des programmes installés avec `dpkg -l`_
- _Installer un paquet spécifique avec `apt-get install`_
