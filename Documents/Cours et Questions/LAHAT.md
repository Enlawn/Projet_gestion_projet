Linux est un système d’exploitation multi-utilisateurs basé sur des permissions. Ce
document a pour objectif d’apprendre à un utilisateur débutant à gérer les fichiers, les
droits d’accès ainsi que les utilisateurs et les groupes.

2 Gestion des fichiers sous Linux
2.1 Le système de fichiers

Sous Linux, tout est organisé sous forme d’arborescence. La racine du système est / .
Répertoires importants :
— /home : dossiers personnels
— /etc : fichiers de configuration
— /var : fichiers variables (logs)
— /bin : commandes essentielles


Les types de fichiers q'ont trouvent generalement sur linux sont 
— - : fichier normal
— d : répertoire
— l : lien symbolique

 Permissions
 Sous linux chaque utilisateur ou groupe ou autres se trouve attribué des droits sur les fichiers .Seul le super-utilisateur a access à tous les fichiers 
Les permissions sont définies pour :
— le propriétaire (user)
— le groupe
— les autres utilisateurs
Droits possibles :
— r : lecture
— w : écriture
— x : exécution (installation d'applications et autres )
Exemple :
- rwxr - xr - -
Dans cet exemple les utilisateurs ont tous les droits(x,w,r),le groupe a le doit de lire(r),et d'execution (x) mais pas d'ecriture(pas de w),les autres ont seulement le droit de lecture (r)

2.5 Modifier les permissions : commande chmod
La commande chmod permet de changer les droits d’accès.
On peut le faire de deux maniere :methode symbolique et methode numerique 

-Methode numerique 
Chaque droit est attribué à un chiffre .
r --->4
W---->2
X---->1

chmod 755 script.sh 
Dans cette exemple on a donne tous les droits à l'utilisateur ,au groupeet aux autres.
— 7=(4+2+1) : lecture, écriture, exécution pour l'utilisateur
— 5=(4+1): lecture et exécution pour le groupe et les autres 

Methode symbolique 
Dans ce cas on doit compredre que :
u=users
g=group
o=others
a=all
+ c'est pour ajouter un droit
- pour supprimer un droit
Exemple:
chmod u+r fichier   on ajoute le droit de lecture au fichier 
chmod g-w fichier   On ajoute le d 'ecrire au fichier 
chmod o+x fichier   On ajoute le d 'éxecution au fichier 
Dans cette exemple on donné de lecture au utlisateurs,supprimer le droit d'ecriture au groupe et donné le droit d'execution aux autres .

Changer le propriétaire : commandes chown et chgrp
chown permet la gestion des utilisatuers et chgrp la gestion des groupes

sudo chown user fichier
Cette commande permet de donner le fichier "fichier"à l'utilisateur user

sudo chgrp groupe fichier
Apres cette commande le fichier "fichier" appartient au groupe "groupe"

2.8 Quiz – Gestion des fichiers
1. Quelle commande affiche les permissions détaillées ?
2. Que signifie le droit x sur un répertoire ?
3. Combien de types de permissions existent ?
4. Que fait la commande chmod ?
5. À quoi correspond la valeur 7 ?
6. Quelle commande change le propriétaire ?
7. Quelle commande change le groupe ?

10. Vrai ou faux : sans x on peut entrer dans un dossier.

3 Gestion des utilisateurs et des groupes
3.1 Notion d’utilisateur
Linux est un système multi-utilisateur. Chaque utilisateur possède :
— un identifiant (UIDID)
— un nom
— un groupe principal
— un dossier personnel
— un shell

3.2 Créer un utilisateur : commande useradd
sudo useradd -m  nom_utilisateur
— -m : crée le dossier personnel(optionnel)

3.3 Définir un mot de passe : commande passwd
sudo passwd nom
Tu met le nom d'utilisateur pour qui tu veux changer le mot de passe 

3.4 Supprimer un utilisateur : commande userdel
sudo userdel nom_utlisateur
sudo userdel -r nom_utilisateur
L'option -r permet de supprimer de dossietr pessonnel de l'utilisateur

3.5 Groupes
Les groupes permettent de gérer les permissions plus facilement.
Prenons par exemple le groupe dev

La commande groupadd permet de creer un groupe et la commande groupdel permet de supprmer un groupe
sudo groupadd dev  
####cette commande creer le groupe appelé dev 
sudo groupdel dev
####cette commande creer le groupe appelé dev 

3.6 Ajouter un utilisateur à un groupe : commande usermod
sudo usermod - aG dev nom_utilisateur
— -a : ajoute sans supprimer les autres groupes dont l'utilisateur appartenait
— -G : groupe secondaire

3.8 Quiz – Utilisateurs et groupes
1. Quelle commande crée un utilisateur ?
2. À quoi sert l’option -m ?
3. Quelle commande définit un mot de passe ?
4. Comment supprimer un utilisateur et son home ?
5. Quelle commande crée un groupe ?
6. Comment ajouter un utilisateur à un groupe ?
8. Où sont stockés les mots de passe ?
9. Un utilisateur peut-il avoir plusieurs groupes ?
10. Vrai ou faux : seul root peut gérer les utilisateurs.
