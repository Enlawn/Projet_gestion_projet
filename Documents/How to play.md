Réflexion sur comment modeler/construire la partie jeu du projet  
On a déjà une base pour le contenu du jeu <=> les scénarios du jeu / les missions que devront réaliser les joueurs  
Mais comment :  
              - Valider une mission  
              - gagner des points   
              - vérifier la maîttrise de la connaissance présenté dans la mission pour passer à la difficulté supérieure  

On a plusieurs axes de développement possible :  
- On peut s'inspirer des applis comme duolingo / Chess / Geoguessr / 
- On peut utiliser le format de Cours + Quizz "classique" -> Squizz/ Kculture  

  Le 1er format sera vraiment interractif : l'utilisateur devra cliquer/écrire / interagir avec le contenu pour répondre  
  Le 2nd format est beaucoup plus simple à implémenter : On explique, de manière textuel, imagé/schématique, par vidéo courte une notion et ensuite à la fin on fait un Quizz qui permet de tester les connaissances vues pendant le cours.  

  Avec le 1er format, il faudra arriver à modéliser, de manière rudimentaire, une interface windows / GNU Linux pour que l'utilisateur puisse directement tester ce qu'il apprend directement sur le site  
  Avec le 2nd format, l'utilisateur devra, tester les compétences montrées directement sur sa machine  
-> le plus simple se baser sur un format Squizz/Kculture, meaning 2eme format -> même pour le site web reprendre une interface similaire avec : quizz d'intro du cours / cours / quizz vérification des acquis  
