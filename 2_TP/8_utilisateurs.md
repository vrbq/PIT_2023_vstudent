_Pour lire cette partie du TP, tu dois :_

- _Avoir arrêter le processus qui faisait dérouler le compte à rebours dans le fichier `sortie.log`_

---

---

Bon, clairement, on ne ré-exécutera plus ce script ! D'ailleurs, allons examiner son ventre parce qu'il ne faudrait pas que d'autres actes malveillants ait été faits sans qu'on s'en aperçoive.

---

<details>
  <summary>  <b> Je n'ai pas la permission pour ouvrir le script .. </b> </summary>

Il te manque alors certainement des droits. Pour voir les droits que possède un fichier, tu peux exécuter la commande `ls -l` :

```
user@debian: ls -l
-rw-r--r-- 1 user group 239 11 sept. 14:04 file
```

Décomposons le résultat de cette commande :

- `-rw-r--r--`: Cette partie représente les permissions du fichier. Elle est composée de 10 caractères :
  - Le premier caractère (le tiret) indique le type de fichier.
    - Ici, il s'agit d'un fichier régulier.
    - Si c'était un répertoire, ce serait un `d` à la place du tiret.
  - Les neuf caractères suivants représentent les permissions. Ils sont divisés en trois groupes de trois caractères chacun.
    - Le premier groupe (`rw-`) indique les permissions du **propriétaire du fichier**.
    - Le deuxième groupe (`r--`) indique les permissions du **groupe auquel appartient le fichier**.
    - Le troisième groupe (`r--`) indique les permissions pour les **autres utilisateurs** (tous les utilisateurs qui ne sont ni le propriétaire ni dans le groupe).

Pour changer les permissions d'un fichier, il faut utiliser commande `chmod`

<details>
  <summary> <b> .. et  je n'ai pas la permission pour modifier les droits .. </b> </summary>

C'est certainement le script que nous avons exécuté qui nous a privé de tous les droits.

Toujours avec `ls -l`, on peut voir le propriétaire du fichier, ainsi que le groupe auquel il appartient :

- `user`: Le nom de l'utilisateur propriétaire du fichier.
- `group`: Le nom du groupe auquel appartient le fichier.

Pour changer le propriétaire et le groupe d'un fichier, il faut utiliser la commande `chown`

Il faudrait donc que `start.sh` t'appartienne à nouveau.
Pour savoir quel nom d'utilisateur tu utilises actuellement, tu peux utiliser la commande `users`.

<details>
  <summary> <b> .. et je n'ai pas la permission pour modifier le propriétaire </b> </summary>

Dans ce cas-là, il faut que tu passes en "super utilisateur". Cet utilisateur, sous Debian, s'appelle couramment `root`. Il faut donc que tu soumettes les commandes de modifications de droits et de propriétaire en mode super utilisateur. Pour cela, deux choix :

- utilises la commande `su - root` pour passer dans l'environnement du super-utilisateur. Tu pourras soumettre tous les commandes avec la permission maximale (les droits sur tout).
- tu peux aussi mettre le mot clé `sudo` avant les commandes que tu soumettre. Cela va exécuter uniquement la commande en mode super-utilisateur, sans te changer d'environnement. Evidemment, il faut que ton utilisateur `user` ait obtenu initialement les droits depuis l'utilisateur `root`.

> _Mais pourquoi on utilise pas `sudo` tout le temps, pour être sûr d'avoir la permission maximale à chaque fois ?_

On se sert de l'utilisateur `root` quand on est sûr de ce qu'on va exécuter ! C'est d'ailleurs ce qui nous a mis dans ce bourbier.
L'utilisateur que nous utilisons, `user`, a la possibilité d'utiliser la commande `sudo`. Par conséquent, les scripts qu'il lance ont aussi cette possibilité !

Un grand pouvoir implique de grande responsabilité, et on ne confie pas les droits administrateurs à tout le monde (comme on confie pas les clés de chez soi à tout le monde).

Pour voir concrètement une différence, vous pouvez tester des commandes destructrices sur votre installation en lecture seule. Par exemple la commande `\rm -rf /`  et `sudo \rm -rf /` n'auront certainement pas le même résultat final... (Pourquoi `\` ?). D'une manière générale on ne travaille jamais en utilisateur root et certains systèmes n'autorisent plus sa connexion. L'usage de la commmande `sudo` doit être limitée aux seuls action modifiant le système : gestion des utilisateurs, gestion des logiciels installés globalement, lancement d'un processus système...
Un processus système est un processus qui peut demande des accès particuliers au noyau (souvent sous la forme d'interruption) ainsi qu'à la couche réseau. Par exemple un utilisateur standard ne peut pas ouvrir un port de communication réseau inférieur à 1024. (Mais il peut de 1024 à 65535, ce qui devrait largement suffire).

</details>

</details>

</details>

Il n'est pas improbable que le script `start.sh` te redirige vers d'autres scripts. Il faudra que tu décomposes tous les scripts et que tu essaies de les comprendre pour voir s'il y a quelque chose de louche qui est apparu.

<details>
  <summary>
   <b> J'ai vu quelque chose de louche ...  </b> </summary>

Mazette, une ligne devrait te perturber : un nouvel utilisateur `hacker` a été créé ! Il vaudrait mieux le supprimer pour ne pas s'exposer à d'autres attaques, au cas où...

La liste de tous les utilisateurs est disponible dans le fichier `/etc/passwd`. De la même manière, la liste de tous les groupes est disponible dans le fichier `/etc/group`

<details>
  <summary> <b> Supprimons cet utilisateur  </b> </summary>

Désormais, il faut supprimer cet utilisateur : `userdel` ou `groupdel` devrait bien t'aider.
Peut-être tu devras utiliser le super utilisateur ?

Penses à vérifier que l'utilisateur est bien supprimé du fichier `/etc/passwd` et `/etc/group`.

</details>

</details>

---

---

_A la fin de cette partie, tu devrais maitriser comment :_

- _Voir les utilisateurs & les groupes d'un système UNIX dans les fichiers `/etc/passwd` et `/etc/group`_
- _Comprendre l'intérêt du super-utilisateur, ses usages et ses risques_
- _Supprimer un utilisateur / groupe_
