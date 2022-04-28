# SPA

## Définition 

### Let

__let nomVariable =__ 
- peut être locale ou globale
- __on peut modifier la valeur plus tard dans le code__ 
- sa potée est limité au bloc où elle est déclarée
- instancier 0 à n fois
- on ne peux pas redéclarer la même variable dans un seul bloc


## Const

__const nomVariable =__ 
- __l'identifiant ne peut pas être réaffecté, valeur reste la même, impossible d'avoir une fonction où variable qui porte le même nom !=__
- peut être locale ou globale
- sa potée est limité au bloc où elle est déclarée
- __doit être initialisé__
- __impossible de changer la valeur plus tard__
-  on peut l'instancier 0 à n fois
-  Tableau = on peut modifier les valeurs tant qu'on ne le réasigne pas. On peut changer ses valeurs en l'appelant avec des index ou rajouter et supprimer des éléments.
- Objet = on peut modifier, supprimer des attributs mais on ne peut pas les réasigner non plus.


## import / export

https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Statements/export

dans function.js :
export const hello = () => console.log('hello');

dans script.js : 
import {hello} from './functions.js';
+
hello();

## this 

### Libre

This va chercher le parent le plus proche si il n'est pas dans un objet (le parent de tous les objets)

## stricte

Non défini ou objet courant

## Composant 

__Instances de vues qui sont réutilisables dans le code autant de fois qu'on veut. Une brique qui va permettre de construire la page en html. Il englobe le HTML avec  template, une partie js qui permet de gérer l'initialisation, les intéractions, la relation entre parent et enfant etc... avec script et le css qui permet d'avoir son style. __

- on peut manipuler des listes avec un composant
- il peut hérité des composants parents

## Particularité de vue.js

Utilise des composants pour créer la page html. Au lieu de modifier tout le dom, vue js va avoir un dom virtuel où tous les changements seront fait. Ensuite, le dom virtuel sera comparé avec le dom existant et il va remplacer les parties du dom qui sont différentes du dom virtuel.

