Voici un résumé des commandes UNIX utilisées lors de ce TP :

### 1 - Boot & Wifi

- `ip link` : Cette commande en UNIX est utilisée pour afficher et gérer les interfaces réseau du système. Elle permet de lister les interfaces réseau disponibles et d'obtenir des informations sur leur statut.

- `cat` : La commande `cat` est utilisée pour afficher le contenu d'un fichier texte à la sortie standard. Elle est souvent utilisée pour lire le contenu des fichiers texte dans le terminal.

- `./script` : Cette commande est utilisée pour exécuter un script ou un programme exécutable présent dans le répertoire courant en spécifiant le chemin relatif, précédé de "./". Par exemple, si vous avez un script nommé "script" dans le répertoire actuel, cette commande l'exécutera.

- `sh ./script` : Cette commande utilise le shell (sh) pour exécuter un script spécifié en utilisant le chemin relatif. Cela peut être utile si le script nécessite un shell spécifique pour son exécution.

- `vi` : La commande `vi` est un éditeur de texte en mode terminal très puissant. Elle permet de créer, modifier et enregistrer des fichiers texte directement depuis le terminal. C'est un éditeur en mode texte complet qui offre de nombreuses fonctionnalités pour l'édition de fichiers.

### 2 - ISO

- `wget` : La commande `wget` est utilisée pour télécharger des fichiers depuis le Web en utilisant le protocole HTTP, HTTPS ou FTP. Elle est souvent utilisée pour récupérer des fichiers ou des ressources à partir d'URL spécifiques.

- `curl` : La commande `curl` est également utilisée pour effectuer des requêtes HTTP, HTTPS ou FTP, mais elle peut également être utilisée pour transférer des données vers un serveur. Curl est un outil polyvalent pour le transfert de données sur le réseau.

- `df` : La commande `df` permet d'afficher l'utilisation de l'espace disque sur le système de fichiers. Elle montre l'espace total, l'espace utilisé et l'espace disponible pour chaque système de fichiers monté.

- `du` : La commande `du` est utilisée pour afficher la taille des répertoires et des fichiers dans le système de fichiers. Elle est utile pour déterminer l'espace disque utilisé par des fichiers et des répertoires spécifiques.

### 3 - ISO

- `mkdir` : La commande `mkdir` est utilisée pour créer un nouveau répertoire (dossier) dans le système de fichiers.

- `mount` : La commande `mount` est utilisée pour monter un système de fichiers ou un périphérique de stockage dans l'arborescence du système de fichiers. Cela permet d'accéder aux données stockées sur ce périphérique.

- `cd` : La commande `cd` est utilisée pour changer de répertoire courant dans le système de fichiers. Elle permet de naviguer entre les répertoires.

- `cp` : La commande `cp` est utilisée pour copier des fichiers et des répertoires d'un emplacement à un autre dans le système de fichiers.

### 4 - EXECUTE

- `ls` : La commande `ls` est utilisée pour lister les fichiers et les répertoires dans le répertoire courant. Elle affiche le contenu du répertoire.

- `chmod` : La commande `chmod` est utilisée pour modifier les permissions d'accès aux fichiers et aux répertoires. Elle permet de définir qui peut lire, écrire ou exécuter un fichier ou un répertoire.

### 5 - FIND

- `htop` : La commande `htop` est un utilitaire de surveillance des processus en mode texte. Elle affiche une liste des processus en cours d'exécution et fournit des informations détaillées sur l'utilisation des ressources système.

- `find` : La commande `find` est utilisée pour rechercher des fichiers et des répertoires dans le système de fichiers en fonction de critères spécifiques, tels que le nom, la taille, ou la date de modification.

### 6 - ARCHIVES

- `man` : La commande `man` est utilisée pour afficher le manuel en ligne d'une commande ou d'un fichier. Elle fournit des informations détaillées sur l'utilisation et les options disponibles.

- `mv` : La commande `mv` est utilisée pour déplacer ou renommer des fichiers et des répertoires dans le système de fichiers.

- `tar` : La commande `tar` est utilisée pour créer, extraire et gérer des archives tar. Elle permet de regrouper des fichiers et des répertoires dans un seul fichier d'archive.

### 7 - PROCESSUS

- `rm` : La commande `rm` est utilisée pour supprimer des fichiers et des répertoires du système de fichiers.

- `rmdir` : La commande `rmdir` est utilisée pour supprimer des répertoires vides du système de fichiers.

- `ps aux` : La commande `ps aux` est utilisée pour afficher une liste détaillée des processus en cours d'exécution sur le système, y compris leur ID, leur utilisation de la CPU, etc.

- `grep` : La commande `grep` est utilisée pour rechercher des chaînes de caractères dans des fichiers ou des flux de texte. Elle permet de filtrer et de manipuler des données textuelles.

- `|` : Le caractère pipe `|` est utilisé pour rediriger la sortie d'une commande vers l'entrée d'une autre commande. Il permet de chaîner des commandes ensemble pour effectuer des opérations complexes.

- `kill` : La commande `kill` est utilisée pour envoyer des signaux à des processus en cours d'exécution, ce qui permet de les arrêter ou de les gérer.

### 8 - UTILISATEURS

- `ls -l` : Cette commande affiche une liste détaillée des fichiers et des répertoires dans le répertoire courant, y compris les informations sur les permissions, le propriétaire, le groupe, la taille, et la date de modification.

- `chown` : La commande `chown` est utilisée pour changer le propriétaire d'un fichier ou d'un répertoire dans le système de fichiers.

- `su - root` : Cette commande est utilisée pour passer à l'utilisateur root en ouvrant une nouvelle session de shell. L'utilisateur root a des privilèges administratifs sur le système.

- `sudo` : La commande `sudo` est utilisée pour exécuter des commandes avec des privilèges administratifs temporaires. Elle permet à un utilisateur autorisé d'exécuter des commandes en tant que superutilisateur (root).

- `userdel` : La commande `userdel` est utilisée pour supprimer un utilisateur du système.

- `groupdel` : La commande `groupdel` est utilisée pour supprimer un groupe d'utilisateurs du système.

### 9 - VENGEANCE

- `umount` : La commande `umount` est utilisée pour démonter (détacher) un système de fichiers monté précédemment à l'aide de la commande `mount`.

- `tail` : La commande `tail` est utilisée pour afficher les dernières lignes d'un fichier texte ou de la sortie d'un flux en temps réel.

- `head` : La commande `head` est utilisée pour afficher les premières lignes d'un fichier texte ou de la sortie d'un flux en temps réel.

### 10 - INSTALL

- `dpkg -l` : Cette commande affiche la liste des packages installés sur le système, y compris leur statut et leur version.

- `apt-get install` : Cette commande est utilisée pour installer des packages sur un système Debian ou Ubuntu en utilisant le gestionnaire de paquets `apt`.

### 12 - BASH

- `echo` : La commande `echo` est utilisée pour afficher du texte ou des variables dans le terminal.

- Variable en bash `$nom` : Les variables en bash sont utilisées pour stocker des valeurs. `$nom` est un exemple de nom de variable.

- Boucle `for` en bash : Une boucle `for` en bash est utilisée pour itérer sur une liste de valeurs ou d'éléments et exécuter des commandes pour chaque élément de la liste.

- Condition `if` en bash : Une condition `if` en bash est utilisée pour exécuter des commandes en fonction d'une condition spécifique. Elle permet de prendre des décisions dans les scripts bash en fonction de l'évaluation d'une expression conditionnelle.

### 13 - END

- Installation d'un paquet en `tar.gz`

  - `./configure` : La commande `./configure` est souvent la première étape de l'installation d'un logiciel à partir de son code source. Elle configure le logiciel en fonction du système sur lequel il est installé, générant des fichiers de configuration adaptés.

  - `make` : La commande `make` est utilisée pour compiler le code source d'un logiciel après avoir configuré les options avec `./configure`. Elle génère les fichiers binaires exécutables à partir du code source.

  - `sudo make install` : Cette commande est utilisée pour installer le logiciel compilé dans le système. Elle copie les fichiers binaires et les ressources associées dans les répertoires appropriés du système de fichiers. L'utilisation de `sudo` est courante car l'installation peut nécessiter des privilèges administratifs pour écrire dans des répertoires système.
