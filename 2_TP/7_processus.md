
*Pour lire cette partie du TP, tu dois :*
- Avoir décompressé l'archive `.defuseInstructions.tar.gz`
---
---

<details>
  <summary>Après avoir décompressé l'archive, je fais quoi ? </summary>

Tu devrais te retrouver avec deux fichiers, encore cachés ! :

```
> ls -a
.processToFind  .defuseManual
```

Même s'ils sont cachés, tu peux tout de même les lire.


</details>

---

<details>
  <summary> Trouver le nom du processus "virus"</summary>

- Le fichier `.processToFind` sert apparement à retrouver le nom du processus qu'il faut arrêter.
  - Il faut jouer sur la présence ou non de fichiers / dossiers.
  - Tu auras besoin des commandes :
    - `rmdir`,`mkdir` `rm`, `ls` et ses options
  - Si tu suis toutes les étapes, tu devrais trouver un mot caché...


</details>



<details>
  <summary>Trouver le PID d'un processus </summary>


- Le fichier `.defuseManual` nous indique comment l'arrêter sans faire "exploser" le virus.
  - On a vu précedemment la commande `htop` qui permet de faire apparaître tous les processus. Il existe aussi la commande `ps aux`. La finalité est la même (affichage des processus courants), mais pas la manière :
    - `htop` lance une supervision des processus dans la fenêtre courante
    - `ps aux` est une commande
  - On peut rediriger la sortie de la commande `ps aux` et la combiner avec la commande `grep` qui permet de rechercher des motifs (patterns) dans du texte.
    - Pour rappel, pour rediriger la sortie de la commade `A` vers une commande `B`, il faut faire : `A | B`

</details>

<details>
  <summary>Désamorcer le "virus"</summary>

Si tout ce passe bien, tu devrais retrouver le nom du processus associé à un numéro : c'est ce qu'on appelle le **PID** (Process Identity).

> Le PID, c'est un numéro unique attribué à chaque processus en cours d'exécution sur un système d'exploitation.

On peut donc gérer l'état d'un processus grâce d'un processus :
- pour arrêter un processus : `kill <PID>`
- pour mettre en pause un processus : `kill -STOP <PID>` ou `pause <PID>`
- pour reprendre un processus mis en pause : `kill -CONT <PID>`

</details>

Penses à bien suivre les instructions donnés par l'auteur du virus !
On se retrouve quand tu as réussi à déjouer le virus !

---
---
*A la fin de cette partie, tu devrais maitriser comment :*
- *Manipuler les fichiers & dossiers avec  `rmdir` / `mkdir` / `rm`*
- *Utiliser les options de `ls` pour trier selon un ordre précis les fichiers*
- *Rediriger la sortie d'une commande vers une autre commande grâce à `|`*
- *Utiliser `grep` pour rechercher un pattern dans du texte*
- *Gérer l'état d'un processus, le mettre en pause & l'arrêter avec `kill` et `pause`*
