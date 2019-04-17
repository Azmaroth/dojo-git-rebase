# Dojo Git Rebase

## Introduction

Ceci est le projet qu'il faudra utiliser lors du Dojo Git Rebase

## Getting Started

TODO:

1. Cloner ce repository
2. Rien d'autre, suivre les exercices au fil des slides

## Exercice 01 - Stash

En local:

1. Modifier un fichier du Repo
2. Faites un `git stash`
3. Créez un nouveau fichier
4. Faites un `git stash`
5. Listez les stashs en cours
6. Restaurez le premier stash créé

## Exercice 02 - Rebase Simple (sans conflit)

1. Depuis `training/<date du jour>-ex2`, créez une branche `votrenom`
2. Effectuez plusieurs commits en créant/modifiant des fichiers
3. Attendez que le formateur crée de nouveaux commits sur `training/<date du jour>-ex2`
4. Récupérez ces modifications à l'aide d'un `rebase`
5. Poussez cette mise à jour sur l'origine

## Exercice 03 - Rebase Simple (avec conflit)

1. Tirez une branche `rebase_votrenom` partant de `training/<date du jour>-ex3`
2. Dans le fichier time.txt :
   - Mettez l’heure à jour
   - Ajoutez, en-dessous, le commentaire « Commit C »
3. Commitez avec le commentaire « C »
4. Réitérez en changeant « C » par « D »
5. Attendez que le formateur crée deux commits `E` & `F` sur la branche `training/<date du jour>-ex3` en changeant l’heure
6. A l’aide d’un rebase, récupérez ces modifications et résolvez les conflits pour obtenir les commits dans l’ordre A, B, E, F, C, D
7. Poussez cette mise à jour sur l'origine

## Exercice 04 - Rebase Interactif

Tirez une branche `rebase-i_votrenom` partant de `training/<date du jour>-ex4`.

### Partie A - Ordre des commits

A l’aide d’un rebase, changez l’ordre des commits pour obtenir A, B, C, D, E, F

### Partie B - Reword

A l’aide d’un rebase intéractif, changez le commentaire de l’avant-dernier commit

### Partie C - Edit

A l’aide d’un rebase intéractif, éditez le commit `C` (modifiez un fichier ou créez-en un)

### Partie D - Squash, Fixup et Drop

A l’aide d’un rebase intéractif :

1. Fusionnez les commits `C` et `D` en modifiant le message du commit
2. Fusionnez les commits `A` et `B` sans modifier celui-ci
3. Supprimez le commit `F`

### Finalement

Poussez vos dernières mises à jour sur l'origine