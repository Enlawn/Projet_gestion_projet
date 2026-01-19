# Commande CMD Windows  
  
On les utilises énormement sur Linux, mais on peut retrouver leurs équivalents sur Windows, une petite présentation des lignes de commande sur Windows.
La plupart des utilisateurs Windows, MacOS et ChromeOS n'utiliseront jamais l'invite de commande (CMD), le Terminal ou l'interface PowerShell. Pourquoi ? Parce que nous en avons pas besoin. Les modifications et fonctionnalités qu'elles proposent sont complétement couvertes par d'autres applications à l'utilisation bien plus simple come l'explorateur de fichier, le panneau de configuration... etc.
Mais, cela ne veut pour autant pas dire qu'ils sont complétement obsolètes, ils restents des outils puissants qui ont aussi un intérêt pédagogique parce qu'ils permettent de mieux comprendre le rôle du système d'exploitation.  
Au passant, si vous devez traiter de nombreux fichiers et dossiers, PowerShell est un outil qui peut vous permettre d'automatiser vos taches "RÉPÉTITIVE".  

Comment accéder à l'inviter de commande ?
MENU DEMARRER -> TAPER "cmd" DANS LA BARRE DE RECHERCHE.  

Il existe différents types de lignes de commande répartis en plusieurs catégories :  

- gestion des fichiers et répertoires,
- gestions des disques,
- commandes système,
- gestions des utlisateurs,
- etc... .

Vous trouverez une très grande quantité de tutoriel et cours qui vous présonteront en détails l'étendu des commandes windows existantes.
Le lien vers un cours fourni directement par Microsoft : <https://learn.microsoft.com/fr-fr/windows-server/administration/windows-commands/windows-commands>
Je vais me contenter de vous présenter celle concernant la gestion des fichiers et répertoires et des commandes système utile.  
je vais, très fortement m'inspirer de l'aide mémoire du site malekal.com et de celui de TechAbeille.fr  .  

Parce que, s'il est possible de demander de l'aide, il est utile de savoir comment faire, il existe des commandes qui permettent d'expliquer le fonctionnement d'une commande :  

- [comande] /?
- help
- help [commande]
  
**1. gestion des fichiers et des répertoires**  
  
dir  
Permet d'afficher  les fichiers et dossiers présent à l'adresse actuelle.  
  
dir [chemin d'accès]  
Permet d'afficher tous les fichiers et dossiers présent à l'adresse pointée par le chemin d'accès.  

dir /o:s [chemin d'accès]  
Affiche tous les fichiers et dossiers présent à l'adresse pointée par le chemin d'accès en les triant par taille.  

dir /o:d [chemin d'accès]  
Affiche tous les fichiers et dossiers présent à l'adresse pointée par le chemin d'accès en les triant par date.  

dir /a [chemin d'accès]  
Affiche tous les fichiers et dossiers, même ceux cachés présent à l'adresse pointée par le chemin d'accès.  

dir /b [chemin d'accès]  
Affiche uniquement les noms de tous les fichiers et dossiers présent à l'adresse pointée par le chemin d'accès.  

---

cd [chemin d'accès]  
Permet de se déplacer vers l'adresse pointée par le chemin d'accès.  

cd ..  
Permet de remonter d'un niveau.  

cd \  
Permet de remonter à la racine du lecteur courant.  

---

mkdir [nom du dossier]  
Crée un dossier dans le répertoire en cours d'utilisation.  

md [nom du dossier]  
Crée un dossier dans le répertoire en cours d'utilisation.  

move [source] [destination]  
Deplace un dossier/fichier.  

---

rmdir [nom du dossier]  
Supprime le dossier.  

rmdir /s [nom du dossier]  
Supprime le dossier et tout les fichiers qu'il contient.  

rd  [nom du dossier]  
Supprime le dossier.  

rd /s [nom du dossier]  
Supprime le dossier et tout les fichiers qu'il contient.  

rd /q [nom du dossier]  
Supprime le dossier sans demander de confirmation, sans les déposer dans la corbeille !  

rd /s /q [nom du dossier]  
Supprime le dossier et tout les fichiers qu'il contient sans demander de confirmation et surtout, sans les déposer dans la corbeille !  

del [nom du fichier.type]  
Supprime le fichier.  

del *[.type]  
Supprime tous les fichiers qui sont du type spécifié.  

---

robocopy [source] [destination]  
Copie robuste avec reprise et synchronisation / alternative + flexible que l'historique copy.  
Propose beaucoup (trop) d'option de copie :  

robocopy [source] [destination] /s  
Ne copie que les répertoires non vides.  

robocopy [source] [destination] /e  
Copie tous les répertoires et fichiers.  

robocopy [source] [destination] /l  
Pas de copie, répertorie les fichiers qui seraient concernés par une demande de copie.  

robocopy [source] [destination] /t  
Copie uniquement les répertoires, sans les fichiers qu'ils contiennent.  

robocopy [source] [destination] /t /e  
Copie uniquement les répertoires, même ceux qui sont vides, sans les fichiers qu'ils contiennent.  

robocopy [source] [destination] /lev:<n>  
Copie que jusqu'au niveau 'n' spécifié.  

robocopy [source] [destination] /mir  
Copie tous les répertoires et fichiers ainsi que leurs paramètres de sécurités.  

robocopy [source] [destination] /move  
Copie tout les répertoires et fichiers vers la destination et les supprime de la source (équivalent du Couper Coller).  

ren [ancien nom] [nouveau nom]  
Renomme le fichier ou dossier.  

---

**2. Commandes système**  

ipconfig  
Affiche l'interface réseau.  

netsh wlan show profile  
Affiche les réseaux WiFi enregistrés sur l'ordinateur.  

whoami  
Affiche le nom de l'utilisateur actuellement connecté

shutdown [options]  
Arrête l'ordinateur selon les options spécifiées :  

- /s arrête l'ordinateur,
- /r redemarre l'ordinateur,
- /t [sec] définit un délai avec arrêt,
- /a annule un arrêt en cours.
  
tasklist  
Répertorie tous les processus en cours (gestionnaire des tâches).  

taskkill /IM [nom du programme]  
Termine un processus dont on a spécifié le nom du programme qui l'exécute.  

systeminfo  
Affiche les informations détaillées du systèmes.  

driverquery  
Affiche les pilotes installés, avec la date d'installation et l'état du pilote.  

sfc /scannow  
Permet d'effectuer un diagnostique des fichiers systèmes windows et les réparer s'ils sont corrompus.  

En dehors des cours, ou pour faire de la partition de disque, je n'ai jamais utilisé les lignes de commandes. Pour chaque ligne de commande présenté, il existe une application qui permet, en un clique de faire la même chose.
Mais dépendement de la plateforme sur laquelle vous travaillez, les lignes de commandes peuvent devenir nécessaire voire obligatoire à connaître (cf les utilisateurs Linux).

---

## Questions
  
Quelle commande crée un dossier ?  

- new
- mkdir
- create
- folder
  
Quelle commande supprime un fichier ?  

- erase
- remove
- del
- rd
  
Quelle commande permet de renommer un fichier ?  

- rename
- mv
- ren
- edit
  
Que fait ipconfig ?

- Gère les fichiers
- Affiche la configuration réseau
- Supprime les connexions
- Installe un pilote
  
Quelle commande affiche l’utilisateur connecté ?  

- user
- who
- whoami
- login
  
À quoi sert tasklist ?  

- Supprimer des tâches
- Lister les processus en cours
- Démarrer un programme
- Nettoyer la mémoire
  
Quelle commande arrête l’ordinateur ?  

- shutdown /s
- poweroff
- stop
- halt
  
Quelle commande affiche les informations système ?  

- sys
- info
- systeminfo
- winver
  
sfc /scannow sert à :  

- Supprimer des fichiers
- Scanner et réparer Windows
- Mettre à jour les pilotes
- Installer un logiciel
  
Vous êtes dans C:\Users\Vina\Documents. Vous tapez **cd..**, dans quel répertoire vous trouvez vous maintenant ?  

- C:\
- C:\Users\Vina
- C:\Users\
- C:\Users\Vina\Documents
  
Quelle commande est la plus dangereuse, car si mal utilisée, elle peut vous faire perdre, **définitivement** vos fichiers ?

- dir
- erase *.txt
- rd /s /q
- move
  
Quelle commande permet de tester une copie sans rien copier réellement ?

- robocopy [source] [destination] /l
- robocopy [source] [destination] /t
- robocopy [source] [destination] /mir
- robocopy [source] [destination] /move
  
Vous voulez tuer un programme bloqué nommé flemme.exe, quelle commande utiliser ?

- taskkill flemme
- taskkill /IM flemme.exe
- kill flemme
- stop flemme
  
Vous voulez supprimer tous les fichiers .pdf d’un dossier. Quelle commande utiliser ?

- del *.pdf
- del pdf
- rd *.pdf
- erase .pdf
  

---
  
# Pour aller plus loin

J'ai menti !  
Il est parfois obligatoire, pour des cas très rare et très précis, d'utiliser les lignes de commandes en windows.  
L'exemple le plus concret est pour l'installation de python et l'installation de compilateur (par exemple MinGW pour le compilateur GCC C++).
Vous pouvez directement utiliser des IDE (integrated development environment) dans lesquels l'ensemble des outils nécessaire à la programmation sont reunis ou bien programmer à la dur, sans assistance, sur un editeur de texte et faire la compilation à partir de la console et donc en utilisant des lignes de commandes.  

Pour la programmation et le développement, Linux reste l'OS de choix.
Mais, pas besoin d'abandonner Windows pour autant !
Il existe différents logiciels qui permettent de simuler l'environnement Linux sur Windows :  

- les machines virtuelles, qui permettent de créer une version virtuelle d'un ordinateur fonctionnant sous une distribution Linux choisie.
- WSL pour "Windows Subsystem for Linux"

Il peut et il est parfois compliqué d'installer une machine virtuelle.
Il est encore plus compliqué, voir dangereux d'installer à côté de Windows, en **dual-boot** une distribution Linux. Si l'installation n'est pas correctement réalisée, vous pouvez vous retrouvez à devoir réinstaller Windows.
C'est pour cela qu'il existe une alternative **sure**, c'est le logiciel WSL. Comme son nom l'indique, c'est une fonctionnalité de Windows qui va vous permettre d'exécuter un terminal Linux sur Windows.
Pour l'installer, il va falloir utiliser des lignes de commandes.
Pour des Cours et tutoriels complet sur le sujet, voici quelques liens utiles :  
<https://learn.microsoft.com/fr-fr/windows/wsl/>
<https://wiki.etud.insa-toulouse.fr/books/travailler-sur-sa-machine/page/wsl-linux-dans-windows>

Pour la documentation et le dépôt GitHub du logiciel :
<https://wsl.dev/>
<https://github.com/microsoft/WSL>

Je vais quand même vous faire une explication simplifier de l'installation de WSL.  

**Avertissement !**  
*Vous devez être sur une version ultérieure à Windows 10 v.2004 ou sur Windows 11 pour pouvoir utiliser les lignes de commandes que je vais donner.*  
*Les lignes de commandes que je vais présenter permettent une installation rapide de WSL avec une distribution Ubuntu.*  

Sur Powershell ouvert en tant qu'administrateur (clique droit sur l'icone -> exécuter en tant qu'administrateur), entrez :  
wsl --install  
  
cette comande va :  

- activer les composants WSL et Activer la virtualisation dans le BIOS
- télécharger et installer le dernier noyau LInux à jour
- définit WSL 2 comme version par défaut
- télécharger et installer la distribution Linux ubuntu

appuyez sur entrée, ensuite redémarrez l'ordinateur.  

Vous pouvez ensuite afficher la liste des distributions Linux disponible avec la commande :  
wsl.exe --list --online  

et modifier la distribution par défaut avec la commande :  
wsl.exe --install distribution_choisie  

pour pouvoir passer à WSL 2 votre distribution :  
wsl.exe --set-version distribution_utilisée 2  
  
Il vous faudra ensuite créer votre compte utilisateur Unix pour commencer à utiliser WSL.
Voici le lien vers un cours expliquant cela en détail :  
<https://learn.microsoft.com/fr-fr/windows/wsl/setup/environment#set-up-your-linux-username-and-password>  
  
**Il est possible d'installer WSL de façon manuelle**  
**Avertissement**  
*WSL 2 n'est compatible qu'avec les versions de Windows antérieur à la version 1903 de Windows 10 donc si vous voulez l'utiliser, vous allez devoir mettre à jour Windows*
*Vous pouvez néanmoins utiliser WSL 1 avec des anciennes versions de Windows*

Sur Powershell ouvert en tant qu'administrateur (clique droit sur l'icone -> exécuter en tant qu'administrateur)  :  
**1. Activer le sous-système Windows pour Linux**  
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart  

appuyez sur entrée, ensuite redémarrez l'ordinateur.  

Toujours sur Powershell en mode administrateur,  
**2. Activer la fonctionnalité de Machine Virtuelle (virtualisation) si vous voulez et pouvez utiliser WSL 2**
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart  

appuyez sur entrée, ensuite redémarrez l'ordinateur.  

**3. Télécharger le package de mise à jour du noyau Linux**  
Pour les machines fonctionnant avec un processeur intel ou amd, donc en architecture x64 :  
<https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi>
Pour les machines avec des processeurs ARM types snapdragon :  
<https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi>

**4. Définir WSL 2 en version par defaut**
wsl --set-default-version 2

**5. Choisir la distribution voulue**  
wsl.exe --list --online  
wsl.exe --install distribution_choisie  

**6. Créer votre compte utilisateur (identifiant + mot de passe)**  

Et voilà, vous devriez avoir finit l'installation de WSL 2 avec ça.
Pour plus de détail, et dans le cas ou vous rencontrez des soucis pendant l'installation :  
<https://learn.microsoft.com/fr-fr/windows/wsl/install-manual>

Et pour conclure, voici un lien vers le site Microsoft dans lequel est regroupé les ressources Linux chez eux :  
<https://learn.microsoft.com/fr-fr/linux/>  
