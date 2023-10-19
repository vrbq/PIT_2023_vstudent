
*Pour lire cette partie du TP, tu dois :* 
- *Avoir déchiffrer le fichier `trafic.log.nc`*
---
---

Maintenant tu es grand.
Tu as un fichier texte.
Un nom d'utilisateur.

Essaies de trouver une information utile qui pourrait relier tangiblement le nom d'utilisateur à quelque chose d'exploitable !

<details>
  <summary> J'ai cherché mais en fait, qu'est-ce qu'on cherche ? </summary>

On cherche une information qui relie le nom d'utilisateur trouvé précédemment avec quelque chose qui le trahi dans la "vraie" vie. Cela pourrait être :
- son nom
- sa localisation
- son adresse
- son numéro de téléphone
- ...
  
</details>

<details>
  <summary> J'ai trouvé une information solide !  </summary>

Maintenant, tu aimerais certainement remonter cette information à une localisation qui existe ! 
Tu peux installer le paquet `whois` en suivant cette documentation :  

[Whois-5.4.3](https://www.linuxfromscratch.org/blfs/view/svn/basicnet/whois.html)

Tu vas installer le paquet d'une manière différente, grâce au `.tar.gz`.

Tu dois télécharger sur ta machine le paquet : https://github.com/rfc1036/whois/archive/v5.4.3/whois-5.4.3.tar.gz
Pour installer un paquet grâce à une archive `tar.gz`, il y a 3 étapes importantes :
1. `./configure` : n'est pas toujours présent mais permet la configuration sur certain paquet
2. `make` : permet de "builder" et compiler le paquet
3. `sudo make install` : permet de l'installer sur ta machine

Pour plus d'infos : https://linuxconfig.org/how-to-install-tar-gz-file-on-linux

</details>

Il ne te reste plus qu'à utiliser correctement la commande `whois` et de chercher qu'est ce que nous indique cette information ...




---
--- 
*A la fin de cette partie, tu devrais maitriser comment :* 
- *Ouvrir un fichier crypté avec `mcrypt`*
- *Installer un paquet depuis un `.tar.gz`*
