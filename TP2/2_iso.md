_Pour lire cette partie du TP, tu dois :_

- _Avoir booté sur Debian_
- _Avoir réussi à te connecter au WiFi_

---

---

Si tu lis ça, c'est que tu as réussi à te connecter à Internet sur la Debian ! Bravo !

Mémorises bien comment faire parce que tu en auras besoin à chaque fois que tu lances la Debian.

On vient de recevoir un mail du client, je te mets une copie ici :

> **_From :_** [ceo@entreprise.fr](mailto:ceo@entreprise.fr)
>
> **_To :_** [chef.de.projet@insa.fr](mailto:chef.de.projet@insa.fr)
>
> Bonjour,
>
> Je vous recontacte puisque j'ai à nouveau une tâche que je ne sais pas exécuter.
>
> Une agence de publicité m'a envoyé ce matin ce lien :
>
> https://github.com/vrbq/PIT_2023/blob/main/TP2/MISE_EN_SITUATION/pit.iso
>
> Je pense que c'est le film publicitaire qu'il vienne de réaliser pour l'entreprise !
> Mais je n'arrive pas à ouvrir le fichier .iso sur ma machine en Debian.
>
> **Est-ce que vous pouvez l'ouvrir pour moi et me retransmettre le film publicitaire en format .mp4 ?**
>
> Merci d'avance !

Eh bien c'est parti, on va investiguer pour lui !

Avant de télécharger, assures toi que tu as l'espace disponible pour télécharger l'image. En effet, si son iso fait 1To, peut-être qu'il va y avoir un souci !

- Pour savoir de quelle taille est un fichier avant de le télécharger, tu peux utiliser l'option `--spider` de `wget` ou bien l'option `-I` de la commande `curl`.
- Il faut donc que tu compares cette taille à la place restante sur ton disque. Pour cela, tu peux utiliser la commande `df`. Les options `-h` et `-H` peuvent t'être utile.

Si c'est OK de ton côté, tu peux télécharger l'image avec `wget` dans le dossier de ton choix !

Tu peux vérifier que la taille du fichier téléchargé est bien la même que celle que tu avais vu avec `wget` grâce à la commande `du`.

---

---

_A la fin de cette partie, tu devrais maitriser :_

- _La visualisation d'une taille de fichier avec `wget`_
- _Le téléchargement d'un fichier avec `wget`_
- _La visualisation de ton espace disque avec `df`_
- _La visualisation de la taille d'un fichier avec `du`_
