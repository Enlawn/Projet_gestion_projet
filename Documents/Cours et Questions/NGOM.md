Cours d'Introduction à Linux — Partie Utilisateur
Introduction
Linux est un système d’exploitation libre et puissant, très répandu dans les environnements professionnels, scientifiques et serveurs. Contrairement à Windows ou macOS, Linux offre une grande flexibilité et un contrôle avancé sur le système, notamment grâce à son terminal (ou shell).
Dans cette session, nous allons découvrir les commandes essentielles pour naviguer, gérer fichiers et répertoires, et effectuer des opérations courantes sous Linux — en nous appuyant sur des exemples concrets comme ceux présents dans votre mémo.

Les 20 commandes Linux les plus utiles (niveau utilisateur)

1. pwd (Print Working Directory)
Affiche le chemin absolu du répertoire courant.


Exemple :

bash
pwd


2. cd (Change Directory)
Permet de se déplacer dans l’arborescence.

Exemples :

bash
cd /home/utilisateur
cd ..          # Remonter d’un niveau
cd ~           # Aller au répertoire personnel
cd -           # Revenir au répertoire précédent (utile !)


3. ls (List)
Liste les fichiers et répertoires.


Exemples :

bash
ls
ls -l          # Format détaillé
ls -a          # Affiche aussi les fichiers cachés
ls -als        # Combinaison utile (comme sur votre mémo)


4. mkdir (Make Directory)
Crée un répertoire.

Exemple :

bash
mkdir mon_dossier
 
5. cp (Copy)
Copie fichiers ou répertoires.


Exemples :

bash
cp fichier1 fichier2
cp -r dossier1 dossier2   # -r pour copier récursivement


6. mv (Move)
Déplace ou renomme fichiers/répertoires.

Exemple :

bash
mv ancien_nom nouveau_nom


7. rm (Remove)
Supprime fichiers ou répertoires.


Exemples :

bash
rm fichier
rm -r dossier   # Supprime récursivement
rm -f fichier   # Force la suppression sans confirmation


8. cat (Concatenate)
Affiche le contenu d’un fichier.


Exemple :

bash
cat mon_fichier.txt


9. grep (Global Regular Expression Print)
Recherche une chaîne de caractères dans un fichier.
Exemple (inspiré de votre mémo) :

bash
grep 'mot-clé' fichier
grep KCNF resultat.txt


10. nano / vim / kate
Éditeurs de texte en terminal ou interface graphique.
Exemple :

bash
nano monfichier
# ou
kate monfichier   # Éditeur graphique


11. touch
Crée un fichier vide ou met à jour sa date de modification.
 
Exemple :

bash
touch nouveau_fichier.txt

12. chmod (Change Mode)
Modifie les permissions d’un fichier.


Exemple :

bash
chmod 755 script.sh

13. chown (Change Owner)
Change le propriétaire d’un fichier.


Exemple :

bash
chown utilisateur:groupe fichier


14. find
Recherche fichiers/répertoires selon critères.

Exemple :

bash
find /home -name "*.txt"


15. ps (Process Status)
Liste les processus en cours.
Exemple :

bash
ps aux


16. kill
Termine un processus.


Exemple :

bash
kill 1234


17. df (Disk Free)
Affiche l’espace disque disponible.


Exemple :

bash
df -h


18. du (Disk Usage)
Affiche la taille occupée par fichiers/répertoires.


Exemple :

bash
du -sh dossier


19. man (Manual)
Affiche le manuel d’une commande.


Exemple :

bash
man ls


20. history
Affiche l’historique des commandes tapées.

Exemple :

bash
history



Conclusion
Maîtriser ces commandes de base sous Linux vous permettra de gagner en efficacité, en autonomie et en compréhension du système.
Le terminal peut sembler intimidant au début, mais il devient un outil puissant une fois les réflexes acquis.
N’hésitez pas à utiliser man pour explorer les options, et à pratiquer régulièrement dans un environnement de test.

Rappel : Beaucoup de commandes existent aussi avec des interfaces graphiques, mais connaître leur équivalent en ligne de commande est un atout professionnel indéniable, notamment pour l’administration système, le développement ou l’analyse de données.
