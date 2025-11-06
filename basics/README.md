# Module « Basics » – Shell Scripting

Ce dossier regroupe les premiers exercices du module **Shell** de la formation **Holberton School**.  
Il constitue l’introduction aux commandes Unix et à la manipulation du système de fichiers via le terminal.

---

## Présentation

Le but de cette série d’exercices est d’apprendre à se repérer et à agir dans un environnement Linux à l’aide du shell Bash.  
Ces exercices posent les bases nécessaires à la compréhension du fonctionnement du système et à l’écriture de scripts automatisés.

Chaque fichier de ce dossier correspond à un exercice précis demandé par la formation.

---

## Objectifs pédagogiques

À l’issue de ce module, l’étudiant doit être capable de :

- Naviguer dans une arborescence Linux avec les commandes de base (`pwd`, `ls`, `cd`, etc.).
- Créer, déplacer, copier et supprimer des fichiers et répertoires.
- Distinguer les différents types de fichiers et comprendre les liens symboliques.
- Gérer les droits d’accès et comprendre la notion de permissions.
- Rédiger des scripts Bash simples respectant les conventions Holberton (Betty linter).

---

## Contenu du dossier

basics/
├── 0-current_working_directory
├── 1-listit
├── 2-bring_me_home
├── 3-listfiles
├── 4-listmorefiles
├── 5-listfilesdigitonly
├── 6-firstdirectory
├── 7-movethatfile
├── 8-firstdelete
├── 9-firstdirdeletion
├── 10-back
├── 11-lists
├── 12-file_type
├── 13-symbolic_link
└── 14-copy_html

Chaque fichier contient un script Bash répondant à une consigne spécifique du programme Holberton.

---

## Détails des exercices

| Fichier | Description |
|----------|--------------|
| `0-current_working_directory` | Affiche le chemin absolu du répertoire courant. |
| `1-listit` | Liste le contenu du répertoire courant. |
| `2-bring_me_home` | Change le répertoire courant vers le répertoire personnel. |
| `3-listfiles` | Liste les fichiers du répertoire courant au format détaillé. |
| `4-listmorefiles` | Liste tous les fichiers, y compris les fichiers cachés. |
| `5-listfilesdigitonly` | Liste les fichiers en affichant les identifiants numériques des utilisateurs et groupes. |
| `6-firstdirectory` | Crée un répertoire nommé `my_first_directory` dans `/tmp/`. |
| `7-movethatfile` | Déplace un fichier `betty` de `/tmp/` vers `/tmp/my_first_directory/`. |
| `8-firstdelete` | Supprime le fichier `betty` situé dans `/tmp/my_first_directory/`. |
| `9-firstdirdeletion` | Supprime le répertoire `/tmp/my_first_directory/`. |
| `10-back` | Change le répertoire courant pour le précédent. |
| `11-lists` | Liste tous les fichiers, y compris ceux des sous-répertoires, dans un format détaillé. |
| `12-file_type` | Affiche le type du fichier nommé `iamafile`. |
| `13-symbolic_link` | Crée un lien symbolique `__ls__` pointant vers `/bin/ls`. |
| `14-copy_html` | Copie tous les fichiers `.html` manquants ou plus récents vers le répertoire parent. |

---

## Instructions d’exécution

Cloner le dépôt :
[Lien vers le depot](git clone https://github.com/GwenP88/holbertonschool-shell.git)

Se déplacer dans le dossier :
`cd holbertonschool-shell/basics`

Rendre un script exécutable :
`chmod +x nom_du_script`
  
Exécuter le script :
`./nom_du_script`
Tous les scripts ont été conçus pour être exécutés sur un environnement Ubuntu 20.04 LTS avec bash version 5.x.

Contraintes techniques
Chaque script doit commencer par le shebang :
`#!/bin/bash`
Aucune commande non autorisée ne doit être utilisée.
Les scripts doivent être valides et sans erreur de syntaxe.

Chaque fichier doit être exécutable :
`chmod +x nom_du_script`
Le code doit respecter les conventions Holberton et passer le Betty linter.

---

## Bonnes pratiques
Tester chaque commande avant de l’intégrer dans un script.
Vérifier les permissions avant d’exécuter ou de supprimer un fichier.
Commenter les parties importantes du code pour expliquer l’intention.
Toujours sauvegarder avant de modifier un fichier système.
Exécuter les scripts dans un environnement de test avant production.

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
