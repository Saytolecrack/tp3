**Nom :** Baltide Sacha
**Groupe :** C
**Année :** 1ère année
**IUT Le Havre - Cours GIT**

### Compte-rendu TP1 Introduction GIT

1. Configuration de git

	On utilise la commande "git config --list" pour obtenir la configuration
actuelle.

	1.1 Identité

	Pour modifier respectivement le nom d'utilisateur et le mail, on entre :
"git config --global user.name "Sacha Baltide"" et "git config --global
user.email sacha.baltide@etu.univ-lehavre.fr"

	1.2 Editeur

	Pour configurer l'éditeur par défaut : "git config --global core.editor gedit"

	Exercices
	
	On entre à la suite :
-> git config --global user.name "Sacha Baltide"
-> git config --global user.email sacha.baltide@etu.univ-lehavre.fr
-> git config --global core.editor gedit

-> git config --list
On remarque que les informations ont été mises à jour :

user.name=Sacha Baltide
user.email=sacha.baltide@etu.univ-lehavre.fr
core.editor=gedit

-> git config user.name
Retourne : "Sacah Baltide"

-> git config user.email
Retourne : sacha.baltide@etu.univ-lehavre.fr


2. Création d'un dépôt git sur une machine locale

	On crée, tout d'abord un répertoire courseGIT avec la commande : "mkdir courseGIT".
Puis, en se plaçant dans courseGIT, on crée un répertoire tp1.

	On crée le dépôt Git avec : "git init". Un répertoire ".git" a aussi été créé.
	
	2.1. La commande git status
	
	La commande "git status" vérifie les modifications apportées aux fichiers.
	
3. Création d’un fichier texte README.md

	3.1. Gérer les différentes modifications du fichier README.md

	"git status" retourne que le fichier README.md n'est pas encore suivi.
Pour qu'il soit sélectionner, il faut entrer la commande : "git add README.md".
Ensuite, pour le valider, il faut entrer : "git commit -m "Ajoute du fichier README.md"".
"git log" permet de voir les versions enregistrées dans les dépôt, chaque entrée du
log correspond à une version du fichier validé.

3.2. Différencier 3 états / 3 zones / 3 actions

	Dans un dépôt Git, un fichier peut avoir trois états : Modifié, quand il y
a des modifications locales qui ne sont ni validées, ni sélectionnées.
Sélectionné, quand les modifications sont sélectionnées, mais pas validées.
Validé, quand il a été validé et qu'il est synchrone avec le serveur.
	Ces états correspondent à trois zones dans Git : La copie de travail, le système
de fichier local où les fichiers sont modifiés.
La zone de sélection. Ainsi que le dépôt dans lequel les modifications sont
enregistrées sous forme de validations.
	Le passage d'un état à un autre se fait par trois actions : Sélection qui
sélectionne les fichiers pour la validation (git add). La validation qui crée le
commit et l'envoie vers le dépôt (git commit). La récupération qui récupère un
instantané depuis le dépôt vers la copie de travail (git checkout).


4. Gestion de version d’un programme Java

	On créé un répertoire "src" qui contiendra les sources de "Cryptomonnaie.java"
que l'on créera avec touch Cryptomonnaie.java".



Nous avons maintenant créé une nouvelle branche de test.
