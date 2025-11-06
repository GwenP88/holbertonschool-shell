# Module « Init Files, Variables et Expansions » – Shell Scripting

Ce dossier regroupe les exercices du second thème du module Shell de la formation Holberton School.  
Il vise à approfondir la compréhension de l’environnement du shell, des fichiers d’initialisation, des variables, et des expansions dans Bash.

---

## Présentation

Lorsque vous utilisez un shell, plusieurs processus interviennent : les fichiers d’initialisation sont lus, les variables définies, les expansions appliquées, puis les commandes exécutées. Ce dossier permet de formaliser ces notions à travers des scripts pratiques.

---

## Objectifs pédagogiques

À l’issue de cette série d’exercices, vous serez capable de :

- Comprendre le rôle des fichiers d’initialisation (par exemple `.bashrc`, `.bash_profile`, etc.) dans un shell Unix/Linux.  
- Définir et utiliser des variables locales et globales dans vos scripts.  
- Utiliser les expansions de variables, d’arithmétique, et de commandes dans Bash.  
- Appliquer correctement les chemins (`PATH`), alias, et modifications de l’environnement utilisateur.  
- Respecter les conventions de scripts Bash (shebang, permissions, style lisible, conformité à Betty linter).

---

## Contenu du dossier

init_files_variables_and_expansions/
├── 0-alias
├── 1-hello_you
├── 2-path
├── 3-paths
├── 4-global_variables
├── 5-local_variables
├── 6-create_local_variable
├── 7-create_global_variable
├── 8-true_knowledge
├── 9-divide_and_rule
├── 10-love_exponent_breath
├── 11-binary_to_decimal
├── 12-combinations
├── 13-print_float
└── 14-decimal_to_hexadecimal

Chaque fichier contient un script Bash conçu pour répondre à une consigne spécifique de la formation.

---

## Détails des exercices

- **0-alias** : crée un alias pour une commande longue.  
- **1-hello_you** : affiche « Hello » suivi du nom passé en argument.  
- **2-path** : affiche la valeur actuelle de la variable `PATH`.  
- **3-paths** : ajoute un nouveau dossier au `PATH`.  
- **4-global_variables** : crée une variable globale et montre qu’elle est accessible dans un script fils.  
- **5-local_variables** : crée une variable locale dans une fonction et montre sa portée limitée.  
- **6-create_local_variable** : définit une variable locale et affiche sa valeur avant et après modification.  
- **7-create_global_variable** : définit une variable globale à partir d’un script.  
- **8-true_knowledge** : utilise une variable et une expansion pour construire et afficher une phrase.  
- **9-divide_and_rule** : effectue une division simple entre deux variables et affiche le résultat.  
- **10-love_exponent_breath** : applique une expansion arithmétique avec l’opérateur exponentiel.  
- **11-binary_to_decimal** : convertit un nombre binaire en nombre décimal à l’aide d’une expansion.  
- **12-combinations** : utilise des expansions pour générer des combinaisons d’arguments.  
- **13-print_float** : affiche un nombre flottant calculé ou saisi.  
- **14-decimal_to_hexadecimal** : convertit un nombre décimal en hexadécimal à l’aide d’une expansion arithmétique.

## Instructions d’exécution

Clonez le dépôt :
`git clone` 
[lien vers le dépot](https://github.com/GwenP88/holbertonschool-shell.git)

Positionnez-vous dans le dossier du module :
`cd holbertonschool-shell/init_files_variables_and_expansions`

Rendez un script exécutable :
`chmod +x nom_du_script`

Exécutez le script :
`./nom_du_script`

Les scripts sont conçus pour être exécutés sur un environnement Ubuntu 20.04 LTS avec Bash version 5.x.

---

## Contraintes techniques

Chaque script commence par :
`#!/bin/bash`

Aucune commande non autorisée ne doit être utilisée.
Les fichiers doivent être exécutables et ne produire aucune erreur de syntaxe.
Le code doit respecter les conventions de la formation Holberton (indentation claire, pas d’espaces inutiles, commentaires pertinents) et être compatible avec Betty linter.

---

## Bonnes pratiques
Vérifiez toujours la valeur d’une variable avant et après modification.
Limitez la portée d’une variable lorsque cela est possible (local vs global).
Utilisez les expansions ($(( ... )), ${VAR}, $(cmd)) de manière appropriée.
Documentez les segments de script complexes avec des commentaires.
Testez les modifications dans un terminal propre afin d’éviter les variables d’environnement résiduelles.

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
