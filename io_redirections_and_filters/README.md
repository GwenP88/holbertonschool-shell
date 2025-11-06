# Module « I/O Redirections et Filtres » – Shell Scripting

Ce dossier regroupe les exercices du module « I/O Redirections et Filtres » de la formation Holberton School.  
L’objectif est d’apprendre à rediriger les flux d’entrée/sortie, à combiner des commandes par des pipes, à filtrer du texte via des utilitaires Unix, et à automatiser ces opérations via des scripts Bash.

---

## Présentation

Lorsque vous travaillez dans un shell, il est crucial de comprendre comment diriger l’entrée (stdin), la sortie (stdout) et les erreurs (stderr), comment transmettre les résultats d’une commande à une autre à l’aide d’un pipe (`|`), et comment filtrer, trier ou traiter du texte via `grep`, `awk`, `sed`, `cut`, etc.  
Ce dossier propose des scripts qui vous poussent à structurer ces traitements.

---

## Objectifs pédagogiques

À l’issue de ce module, vous serez capable de :

- Utiliser les redirections (`>`, `>>`, `<`, `2>`, `&>`, `<<`) pour diriger les flux d’un script ou d’une commande.  
- Employer des pipes (`|`) pour chaîner des commandes et traiter du texte.  
- Appliquer des filtres standards (`grep`, `cut`, `tr`, `sort`, `uniq`, `wc`, `head`, `tail`) pour extraire ou transformer des données.  
- Écrire des scripts Bash qui combinent redirections et filtres de façon efficace.  
- Respecter les conventions de script Bash (shebang, exécution, lisibilité, conformité au Betty linter).

---

## Contenu du dossier

io_redirections_and_filters/
├── 0-hello_world
├── 1-confused_smiley
├── 2-hellofile
├── 3-twofiles
├── 4-lastlines
├── 5-firstlines
├── 6-third_line
├── 7-file
├── 8-cwd_state
├── 9-duplicate_last_line
├── 10-no_more_js
├── 11-directories
├── 12-newest_files
├── 13-unique
├── 14-findthatword
├── 15-countthatword
├── 16-whatsnext
├── 17-hidethisword
├── 18-letteronly
├── 19-AZ
├── 20-hiago
├── 21-reverse
└── 22-users_and_homes

Chaque fichier contient un script Bash conçu pour répondre à une consigne spécifique du module « I/O Redirections et Filtres ».

---

## Détails des exercices

- **0-hello_world** : affiche « Hello World » via redirection ou script simple.  
- **1-confused_smiley** : utilise une redirection ou un filtre pour afficher un smiley confus.  
- **2-hellofile** : redirige la sortie d’un script dans un fichier `hello` et vérifie son contenu.  
- **3-twofiles** : génère deux fichiers puis traite ou compare leur contenu via un script.  
- **4-lastlines** : extrait les dernières lignes d’un fichier à l’aide de `tail` ou équivalent.  
- **5-firstlines** : extrait les premières lignes d’un fichier à l’aide de `head` ou équivalent.  
- **6-third_line** : affiche uniquement la troisième ligne d’un fichier.  
- **7-file** : identifie ou traite un fichier spécifique via script et redirections.  
- **8-cwd_state** : capture l’état du répertoire courant et le redirige dans un fichier.  
- **9-duplicate_last_line** : duplique la dernière ligne d’un fichier via redirection et filtrage.  
- **10-no_more_js** : supprime ou filtre les fichiers `.js` ou supprime les lignes contenant « .js ».  
- **11-directories** : liste les répertoires uniquement ou traite les répertoires via filtre.  
- **12-newest_files** : affiche les fichiers les plus récents dans un dossier.  
- **13-unique** : affiche les lignes uniques d’un fichier ou filtre doublons via `uniq`.  
- **14-findthatword** : trouve un mot spécifique dans un fichier via `grep` ou `awk`.  
- **15-countthatword** : compte les occurrences d’un mot dans un fichier via `grep -c` ou `wc -l`.  
- **16-whatsnext** : enchaîne plusieurs commandes pour produire un résultat complexe.  
- **17-hidethisword** : supprime ou masque un mot spécifique dans un fichier via `sed` ou `tr`.  
- **18-letteronly** : filtre uniquement les caractères alphabétiques ou supprime les autres.  
- **19-AZ** : trie ou affiche les lettres de A à Z ou traite un fichier pour afficher l’alphabet.  
- **20-hiago** : script personnalisé appliquant redirections et filtres selon consigne.  
- **21-reverse** : reverse le contenu d’un fichier ou d’un flux via `rev`, `tac` ou `awk`.  
- **22-users_and_homes** : liste les utilisateurs et leurs répertoires personnels à partir de `/etc/passwd` ou équivalent.

---

## Instructions d’exécution

Clonez le dépôt :  
`git clone https://github.com/GwenP88/holbertonschool-shell.git`
   
Accédez au dossier :
`cd holbertonschool-shell/io_redirections_and_filters`

Rendez un script exécutable :
`chmod +x nom_du_script`

Exécutez le script :
`./nom_du_script` 

Les scripts ont été conçus pour être exécutés sur un environnement Ubuntu 20.04 LTS avec Bash version 5.x.

---

## Contraintes techniques

Le premier ligne de chaque script doit être :
`#!/bin/bash`

Utiliser uniquement les commandes, options et redirections autorisées par la formation.
Chaque script doit être exécutable sans erreur de syntaxe.
Le code doit respecter les normes de style Holberton (indentation claire, nommage cohérent), et passer le Betty linter.

---

## Bonnes pratiques
Vérifiez la sortie d’un pipe ou d’une redirection avant de l’utiliser dans un script.
Utilisez les redirections pour séparer stdout et stderr quand nécessaire.
Testez les filtres (grep, sed, tr, cut, sort, etc.) sur des fichiers d’essai avant de les intégrer dans un script de production.
Commentez les parties complexes du code pour faciliter la lecture et la maintenance.
Assurez-vous de tester vos scripts dans un environnement similaire à celui de la formation pour éviter les effets inattendus.

---

## Auteur

Gwen Pichot
Étudiante en développement web – [Holberton School](https://www.holbertonschool.fr/)

Haute-Savoie, France
[Profil GitHub](https://github.com/GwenP88)

---

## Licence

Ce projet est publié sous licence MIT.
Tu es libre de l’utiliser, le modifier et le redistribuer tant que la licence d’origine est conservée.

--- 

## Remerciements

Projet réalisé dans le cadre du programme Holberton School – Foundations
“The best way to learn coding is by doing.”

