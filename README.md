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
-  instancier 0 à n fois
-  dans tableau = tant qu'il reste un tableau on peut changer les attributs 
-  objet = on peutchanger les valeurs des propriétés tant qu'on ne les change pas.


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
