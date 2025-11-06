# Holberton School – Shell

> **Module de formation : Shell, Bash & Commandes Unix**

Ce dépôt regroupe l’ensemble des projets et exercices du module **Shell** de la formation **Holberton School**.  
Il a pour objectif d’apprendre à manipuler efficacement le terminal, à automatiser des tâches, et à comprendre le fonctionnement du système Linux à travers le shell Bash.

---

## Sommaire

- [Présentation](#-présentation)
- [Objectifs pédagogiques](#-objectifs-pédagogiques)
- [Arborescence du projet](#-arborescence-du-projet)
- [Exécution des scripts](#-exécution-des-scripts)
- [Contraintes techniques](#-contraintes-techniques)
- [Compétences acquises](#-compétences-acquises)
- [Auteur](#-auteur)
- [Licence](#-licence)
- [Remerciements](#-remerciements)

---

## Présentation

Ce projet fait partie du **tronc commun Holberton School**, et constitue une introduction essentielle à l’environnement Linux.  
L’objectif est de **comprendre les bases du shell Bash**, d’apprendre à écrire des **scripts simples mais robustes**, et de maîtriser les **commandes fondamentales** de gestion de fichiers, de permissions et de redirections.

Chaque dossier correspond à une thématique précise, avec des exercices gradués en difficulté.

---

## Objectifs pédagogiques

- Découvrir et comprendre le fonctionnement du **shell Unix**
- Manipuler les **fichiers et répertoires** depuis la ligne de commande
- Utiliser les **redirections**, les **pipes** et les **filtres**
- Gérer les **permissions** et les **droits d’accès**
- Créer et exécuter des **scripts Bash automatisés**
- Utiliser les **variables**, **expansions** et **commandes intégrées**
- Respecter les **bonnes pratiques de scripting** et la syntaxe Bash

---

## Arborescence du projet

holbertonschool-shell/
│
├── basics/
│   ├── 0-current_working_directory
│   ├── 1-listit
│   ├── 2-bring_me_home
│   ├── 3-listfiles
│   ├── 4-listmorefiles
│   ├── 5-listfilesdigitonly
│   ├── 6-firstdirectory
│   ├── 7-movethatfile
│   ├── 8-firstdelete
│   ├── 9-firstdirdeletion
│   ├── 10-back
│   ├── 11-lists
│   ├── 12-file_type
│   ├── 13-symbolic_link
│   └── 14-copy_html
│
├── init_files_variables_and_expansions/
│   ├── 0-alias
│   ├── 1-hello_you
│   ├── 2-path
│   ├── 3-paths
│   ├── 4-global_variables
│   ├── 5-local_variables
│   ├── 6-create_local_variable
│   ├── 7-create_global_variable
│   ├── 8-true_knowledge
│   ├── 9-divide_and_rule
│   ├── 10-love_exponent_breath
│   ├── 11-binary_to_decimal
│   ├── 12-combinations
│   ├── 13-print_float
│   └── 14-decimal_to_hexadecimal
│
├── io_redirections_and_filters/
│   ├── 0-hello_world
│   ├── 1-confused_smiley
│   ├── 2-hellofile
│   ├── 3-twofiles
│   ├── 4-lastlines
│   ├── 5-firstlines
│   ├── 6-third_line
│   ├── 7-file
│   ├── 8-cwd_state
│   ├── 9-duplicate_last_line
│   ├── 10-no_more_js
│   ├── 11-directories
│   ├── 12-newest_files
│   ├── 13-unique
│   ├── 14-findthatword
│   ├── 15-countthatword
│   ├── 16-whatsnext
│   ├── 17-hidethisword
│   ├── 18-letteronly
│   ├── 19-AZ
│   ├── 20-hiago
│   ├── 21-reverse
│   └── 22-users_and_homes
│
└── permissions/
    ├── 0-iam_betty
    ├── 1-who_am_i
    ├── 2-groups
    ├── 3-new_owner
    ├── 4-empty
    ├── 5-execute
    ├── 6-multiple_permissions
    ├── 7-everybody
    ├── 8-James_Bond
    ├── 9-John_Doe
    ├── 10-mirror_permissions
    ├── 11-directories_permissions
    ├── 12-directory_permissions
    └── 13-change_group

## Exécution des scripts

Cloner le dépôt :
`git clone`
[Lien vers le depot](git clone https://github.com/GwenP88/holbertonschool-shell.git)

Se déplacer dans le dossier du projet :
`cd holbertonschool-shell`

Rendre un script exécutable :
`chmod +x nom_du_script`

Exécuter le script :
`./nom_du_script`
Tous les scripts sont testés sur Ubuntu 20.04 LTS avec bash (version 5.x)

## Contraintes techniques

Interpréteur : #!/bin/bash en première ligne de chaque script
Aucune commande ou option non autorisée ne doit être utilisée
Les fichiers doivent être exécutables et sans erreur de syntaxe
Les scripts doivent respecter le format exigé par Holberton (Betty linter)
Les fichiers ne doivent pas contenir de caractères superflus (espaces, retours inutiles)

## Compétences acquises

Maîtrise des commandes de base (ls, cd, pwd, mv, cp, rm, mkdir, etc.)
Gestion des droits d’accès (chmod, chown, chgrp)
Utilisation des variables et expansions
Redirections d’entrée/sortie et utilisation des pipes
Manipulation de flux texte (grep, cut, tr, sort, uniq, wc, head, tail, etc.)
Création de scripts automatisés
Respect des bonnes pratiques Bash (syntaxe, commentaires, lisibilité)

## Auteur

Gwen Pichot
Étudiante en développement web – [Holberton School](https://www.holbertonschool.fr/)

Haute-Savoie, France
[Profil GitHub](https://github.com/GwenP88)

## Licence

Ce projet est publié sous licence MIT.
Tu es libre de l’utiliser, le modifier et le redistribuer tant que la licence d’origine est conservée.

## Remerciements

Projet réalisé dans le cadre du programme Holberton School – Foundations
“The best way to learn coding is by doing.”

