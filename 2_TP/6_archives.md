
*Pour lire cette partie du TP, tu dois :*
- *Avoir trouvé le fichier `.defuseInstructions.tar.gz`*
---
---

J'étais sûr qu'il avait caché quelque chose pour pouvoir s'en sortir ! Tu as donc trouver un fichier qui s'appelle : `.defuseInstructions.tar.gz`

<details>
  <summary>A quoi sert le '.' devant un fichier / dossier ? </summary>

Pour information, le `.` devant un fichier / dossier sert à cacher ces derniers. Certaines options permettent néanmoins de faire apparaître ces fichiers. C'est le cas par exemple de la commande `ls` et l'option `-a`.

Par ailleurs, il est important que tu saches que certaines commandes atteignent leur plein potentiel en utilisant correctement les options.

Par exemple, voici quelques options de la commande `ls` qui pourrait te servir :

- `-l` : Cette option permet d'afficher une liste détaillée des fichiers et des répertoires, y compris des informations telles que les autorisations, le propriétaire, le groupe, la taille, la date de modification.
- `-S` : Trie les fichiers par taille, en affichant les fichiers les plus volumineux en premier.
- `-r` : Inverse l'ordre de tri, affichant la liste des fichiers en ordre inverse.
- `-R` : Cette option permet d'afficher de manière récursive le contenu des sous-répertoires, en listant les fichiers et répertoires dans les sous-répertoires.
- `-t` : Cette option trie la liste des fichiers par date de modification, affichant les fichiers les plus récents en premier.

Et encore bien d'autres, que je te laisserai découvrir ! Tu peux toujours utiliser la commande `man` qui te donnera la liste détaillée des options.


</details>


---

<details>
  <summary>J'aimerais enlever la propriété "caché" du fichier</summary>

Pour pouvoir le faire **ré**-apparaitre (c-a-d enlever sa propriété "caché"), tu peux renommer le fichier en enlevant le `.` devant. Pour renommer un fichier, utilises la commande `mv`.

</details>

---

<details>
  <summary>C'est quoi un fichier tar.gz</summary>

Ce type de fichier qui finit en `tar`, `tar.gz`, `tbz`, `.zip`, `.jar` ou `.rar`... c'est ce qu'on appelle des **archives**. Elles permettent de plier plusieurs fichiers et dossiers dans un même et seul fichier, souvent compressé (.gz, .zip, z, Z, J).

On va donc avoir besoin de *déplier* et *décompresser* l'archive. Pour cela, tu auras besoin de la commande `tar` et certainement de ses options `-x`, `-f`, `-z` et `v`.

Une fois cela fait, rends toi dans le dossier que tu viens d'extraire et lis le contenu des fichiers.


</details>




---
---
*A la fin de cette partie, tu devrais maitriser comment :*
- *Visualiser les fichiers cachés dans un répertoire avec `ls -a`*
- *Comprendre l'importance des options lors de l'utilisation d'une commande*
- *Renommer un fichier avec `mv`*
- *Déplier / Décompresser une archive avec `tar`*
