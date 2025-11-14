deux fonctionnalités 
git revert permet de revenir en arrière d'un commit en copiant le commit précédent sans "oublier" le commit avec l'erreur que l'on a voulu reprendre
Alors que le git reset déplace la branche au commit précédent à partir du quel on peut corriger notre erreur, il "oublie" le commit que l'on souhaite enlever
Exemple : commit1->commit2   : git revert : commit1->commit2->commit1'->suite
commit1->commit2   : git reset : commit1->suite  (commit2)