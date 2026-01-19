# Paramètrage avancé et Benchmarking

## Les paramètres BIOS : une optimisation avancée mais dangereuse  

Avec la partie paramètres, vous avez pu voir qu'il est possible de personnaliser et paramètrer plein de fonctionnalité de votre ordinateur windows. Mais, vous l'avez peut-être remarqué, les paramètres pour certaines catégories de fonctionnalités sont limité :  

- les paramètres d'alimentation
- les paramètres hardware : vitesses des ventilateurs, de la ram, du cpu
- les paramètres de consommation électrique
- les paramètres de démarrage
  
Tous ces **paramètres, qui, si mal paramètrés peuvent fragiliser l'intégrité des composants voir même empécher l'allumage de l'ordinateur** ne se trouve pas dans la partie utilisateur de windows.  
Ils sont propres à chaque carte mère sur laquelle sont installés les composants faisant fonctionner votre ordinateur.  
  
Mais comment y accéder ?  
Cela dépend du constructeur, mais les touches courantes pour accéder au BIOS sont :

- SUPPR ou DEL
- F2
- F10
- F12
- ESC ou ECHAP
Le plus simple reste de faire une recherche internet pour savoir quelle touche permet d'accéder à votre BIOS.  
L'accès au BIOS se fait uniquement au démarrage, et il faut appuyer (continuement ou rapidement et de nombreuse fois dessus) sur la bonne touche.  
  
On l'a vu avec la migration forcé des ordinateurs windows de W10 vers W11, certains paramètres nécessaire à faire fonctionner la version 11 de Windows doivent être activé dans le BIOS.  
Et une mauvaise manipulation peut vous mettre dans l'embaras, comprenez envoyer l'ordinateur au SAV ^^.  
Mais pas que, dependement de l'équipement que vous possédez, les paramètres par défaut peuvent ne pas être les paramètres optimum : la vitesse des RAM, le mode de consommation electrique de la CM, l'alimentation de votre CPU.  
Tant de paramètres, qui quand vous lancez votre machine pour la première fois peuvent vous faire dire : "Bizarre ça, pourquoi mon ordinateur à 4000 euros ouvre l'explorateur de fichier plus lentement qu'un ordinateur sous Windows vista ?".  
Le BIOS, c'est l'interface graphique de votre carte mère.
Qui veut dire "Basic Input/Output System", il est le premier logiciel que votre ordinateur lance quand vous l'allumez pour la première fois.
C'est dessus que vous allez par exemple spécifier ou se trouve (sur quel disque de stockage) le système d'exploitation que vous allez utiliser et installer.
  
Outre la sensation de lenteur visible, d'autre soucis d'optimisation "basique" peuvent entrainer une mauvaise expérience d'utilisation.  
Mais comment savoir que j'ai un truc qui est mal paramètré, me direz-vous ?  
Faites comme moi, passez des heures à lire la doc de vos composants et à vous perdre sur Reddit et faq des constructeurs de vos composants ?  
Ou bien demander à ChatGPT ou Gemini au risque de ne jamais comprendre ce que vous lisez ?  
Je vous propose une solution autre, qui vous permettra, en plus de connaître les performances de votre ordinateur, de pouvoir apprendre à l'entretenir par vous même et d'avoir une meilleur maîtrise de votre équipement.  
C'est le Benchmarking, mot anglais qui veut simplement dire faire une "analyse comparative à une base standardisée".  
En gros, en va comparer les performances des composants de votre ordinateurs aux performances des mêmes composants chez d'autre personnes et des valeurs fournis par le constructeur. On va donc analyser les performances de notre ordinateur.  
C'est également le meilleur moyen de controler le coût de vos équipements informatiques !  
Et de savoir quand un composant commence à devenir obsolète.  
J'en utilise principalement 2 :  

- Pour l'état général de mon ordinateur, ainsi que la cohérence de mes paramètres : Userdiag <https://userdiag.com/fr/>  
- Voici un exemple de rapport que l'on peut obtenir avec **Userdiag** : <https://userdiag.com/id/GKvOSMIkkd> (userdiag de ma machine)  
Pour les paramètres et performance de ma carte graphique (GPU) : **CineBench** <https://www.maxon.net/fr/cinebench?srsltid=AfmBOop6QD4pVKE-YryYHiDRHLOtseb9TZVAgVgYmNA7Q7ByqLM0oWCI>  
Il en existe plein d'autres types pour des usages précis :  
Si vous avez un processeur Intel, le constructeur propose tout en ensemble de software permettant de paramètrer jusqu'au comportement de chaque coeur du processeur !  
Pareil pour votre carte graphique, le constructeur (amd, nvidia, intel,...) propose des logiciels pour paramètrer minutieusement votre carte graphique.
Pour un "simple monitoring" de vos composants, il existe des solutions gratuite comme **HWMonitor** ou celle fourni par le fabricant de votre Carte Mère (CM).  

C'est super, maintenant vous savez ce que votre machine à dans le ventre, et donc ?  
Qu'est-ce qu'il faut regarder ?  
En soit 3 parties :  

- La **partie BIOS** : savoir si vos drivers et votre version du bios sont à jour, mais surtout, le mode de démarrage, TPM, Secure Boot qui sont les principales raison qui vous empécheront de passer de W10 à W11.
- La **partie Processeur** : le plan d'alimentation (parfois nommé "profil d'alimentation") qui doit être adapté à votre utilisation + les températures de fonctionnement, si vous atteingnez des températures avoisinant les 100°C, outres les économies de chauffage que vous pouvez réaliser, vérifier la ventilation de votre centrale nucléaire, la consommation électrique et la fréquence de fonctionnement vous permettront d'améliorer la situation.
- La **partie Mémoire** : vérifiez absolument que le "profil XMP" est activé ! Par défaut, les barettes de DRAM sont paramètré pour fonctionner à leur fréquence minimale. Il faut donc activer le profil XMP (eXtreme Memory Profile pour les CPU Intel) ou EXPO (si vous avez un CPU AMD) dans le BIOS pour profiter pleinement de votre équipement.  
  
**Je le rappel, pour que vous soyez pleinement conscient des risques, comme indiqué dans le titre, toucher aux paramètres du BIOS reste une manipulation dangereuse, et à moins de pleinement connaître les paramètres que vous modifiez, ne changez au grand jamais des valeurs !**  


---

## Questions  
  
Le BIOS est :

- Un logiciel Windows
- Le premier logiciel lancé au démarrage
- Un pilote graphique
- Une application de benchmark
  
Où se trouvent les paramètres avancés du matériel ?

- Dans les paramètres Windows
- Dans le gestionnaire des tâches
- Dans le BIOS
- Dans l’explorateur de fichiers
  
Une mauvaise configuration du BIOS peut :

- Accélérer Windows
- Endommager les composants
- Supprimer des fichiers
- Installer des pilotes
  
TPM et Secure Boot sont importants pour :

- Jouer
- Passer de Windows 10 à Windows 11
- Augmenter la RAM
- Installer Linux
  
Le BIOS signifie :

- Basic Internal Operating System
- Binary Input Output Software
- Basic Input/Output System
- Boot Interface Operating Software
  
Un utilisateur modifie les tensions CPU sans comprendre ce qu'il fait, que risque-t-il ?  

- Perte de fichiers
- Instabilité ou panne matérielle
- Désinstallation de Windows
- Rien
  
A quoi sert Userdiag ?  

- De modifier le BIOS
- D’analyser les performances globales
- De créer des partitions
- D’installer des pilotes

A quoi sert CineBench  principalement ?  

- Le stockage
- Le réseau
- Le processeur / GPU
- La RAM uniquement
  
HWMonitor sert à :

- Overclocker
- Surveiller températures et tensions
- Mettre à jour Windows
- Modifier le BIOS
  
Le profil XMP concerne quel composant ?

- Le GPU
- La RAM
- Le disque dur
- La carte réseau
  
Par défaut, la RAM fonctionne :

- À sa fréquence maximale
- À sa fréquence minimale
- En mode overclocké
- En mode économie d'énergie maximale
  
EXPO est l’équivalent XMP pour :

- Intel
- Nvidia
- AMD
- Qualcomm
  
Une température CPU proche de 100°C indique :

- Un fonctionnement optimal et des économies de chauffage
- Un problème potentiel de refroidissement
- La possession d'un CPU des générations maudites 13 et 14 d'Intel
- Un bug graphique du logiciel de surveillance
  
Le plan d’alimentation de l'ordinateur influence :

- La résolution d’écran
- Les performances et la consommation
- Le stockage
- Le BIOS
  
De quoi dépend le BIOS ?

- Du système Windows
- De la carte mère
- Du disque dur
- Du compte utilisateur
  
Quel est le BON réflexe avant toute modification avancée du BIOS ?  

- Modifier plusieurs paramètres
- Noter les valeurs d’origine
- Lancer un jeu
- Mettre à jour Windows
  
---

