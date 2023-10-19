Hello !

Aujourd'hui, je viens d'avoir le client au téléphone, il a une nouvelle problématique et nous transfère un mail dans quelques minutes.

Tu te rappelles la dernière fois, on avait monté une clé USB qui permettait de booter directement sur un environnement UNIX : Debian.

Lors de la prochaine séance, tu seras directement en face à face avec le client, et tu devras lui montrer que tu maitrises pour pouvoir lui faire accepter cette solution pour lui et ses employés.

Donc pour commencer, je vais te demander de booter sur cette clé USB !

Une fois que tu as booté, tu devras activer le Wifi. Pour cela :

1. Trouve le fichier : `demarrage-eduroam.sh`
2. Affiche le fichier avec `cat`
3. Edite les champs demandés dans le fichier avec `vi` (voir le tutoriel ci-dessous) :
   1. Ton nom d'utilisateur : `p.nom` avec `p` la première lettre de ton prénom
   2. L'interface Internet que tu peux trouver avec la commande `ip link`
4. Décommentes les deux dernières lignes (en supprimant le caractère `#`)

Enfin, pour finir, il faut que tu lances le script.

Je sais que c'est une des deux commandes, mais je ne sais plus laquelle :

- `sh ./script.sh`
- `./script.sh`
  Recherche la différence entre les deux et utilises celle que tu penses la bonne.

Après avoir activé le Wi-Fi, tu peux te rendre à la prochaine étape.
Pour cela, rends toi sur le lien suivant :

(disponible aussi en version courte :)

--- A propos de `vi` ---

Je pense que tu te rendras vite compte que `vi` n'est pas si simple à maitriser si tu ne t'en es jamais servi, alors voilà quelques règles essentielles !
Bien sûr, tu peux t'aider d'Internet sur une autre machine qui elle, est connectée;
`vi` est un éditeur de code de programmation. Il a donc un comportement optimisé pour éditer du code. Par rapport à du code machine, il fonctionne selon deux modes. Un mode permetttant de manipuler les lignes, le mode 'Normal', un mode permettant de saisir des lignes, le mode 'Insertion'.

- **Ouvrir un fichier :** Pour ouvrir un fichier avec `vi`, tapez `vi` suivi du nom du fichier à éditer. Par exemple : `vi mon_fichier.txt`

- **Sortir à tous les coups sans sauvegarder :** Tapez les 5 touches suivantes les unes derrière les autres.
  `<ESC><ESC>:q!`

- **Modes de vi :**

  - **Mode Normal :** Lorsque vous ouvrez un fichier avec `vi`, vous êtes toujours en mode normal. Vous ne pouvez pas éditer le texte dans ce mode, mais vous pouvez effectuer des opérations telles que la _navigation_ et la manipulation de lignes ou de code de code comme la _suppression_, le _remplacement_ ou la _copie_.
  - **Mode Insertion :** Pour entrer en mode insertion et commencer à éditer le texte, appuyez sur la touche `i`.
    - Vous pouvez alors désormais éditer du texte.
    - Vous pouvez également utiliser d'autres commandes pour entrer en mode insertion, comme `a` (après le curseur) ou `I` (au début de la ligne).

- **Navigation :**

  - En mode _normal_, utilisez les touches de déplacement pour vous déplacer dans le texte.
  - Par exemple, `h` (gauche), `j`(bas), `k` (haut), `l` (droite). Vous pouvez aussi utiliser `w` pour avancer d'un mot et `b` pour reculer d'un mot.

- **Suppression :**

  - En mode _normal_, utilisez `x` ou `Suppr` pour supprimer le caractère sous le curseur.
  - Pour supprimer une ligne entière, utilisez `dd`.
  - Pour supprimer plusieurs lignes, utilisez `Ndd`, où `N` est le nombre de lignes à supprimer.

- **Enregistrement et sortie :**
  - Pour quitter `vi` sans enregistrer, revenez en mode normal et tapez `:q!` puis appuyez sur `Entrée`.
  - Pour enregistrer et quitter, revenez en mode normal et tapez `:wq` puis appuyez sur `Entrée`.

---
