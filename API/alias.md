# Documentation d'Alias - API I/O

Alias est une API permettant de créer de stocker des clés et leur valeur de remplacement. Vous pouvez stocker tout type de valeur de remplacement, cela inclut les expressions régulières.

## Accès
L'API Alias est disponible à cette adresse: [https://api.dvp.io/alias/](https://api.dvp.io/alias/)

## Paramètres
* **sid** string alnum
> Session permettant de vous identifier auprès du serveur, cette session permet de retrouver les alias spécifiques à un utilisateur (variable session du chat)

* **key** string alpha
> Clé de l'alias qui sera remplacée par la valeur

* **value** string *
> Valeur de remplacement pour l'alias

## Utilisation

Pour créer/remplacer un alias il suffit d'indiquer la clé accompagnée de sa valeur, pour supprimer un alias il suffit de renseigner la clé sans sa valeur. Pour supprimer tous les alias vous pouvez utiliser le wildcard * 
sans indiquer de valeur.

### Création/modification d'un Alias
```
https://api.dvp.io/alias/?sid=session&key=toto&value=tata
```
La valeur de l'alias `toto` prend `tata` pour valeur

### Supression d'un Alias
```
https://api.dvp.io/alias/?sid=session&key=toto
```
L'alias `toto` viens d'être supprimé


### Supression de tous les Alias
```
https://api.dvp.io/alias/?sid=session&key=*
```
Tous les alias existants ont étés supprimés

## Les alias par défaut
Suite à certains changements cette API fournit une liste d'alias prédéfinis, ces alias sont les mots SMS qui sont interdits sur le chat. Ceci vous permet de les intégrer à votre application cliente afin de faire de 
la prévention aurpès de vos utilisateurs. Cette liste est suceptible d'avoluer régulièrement, il est donc fortement conseillé de la mettre à jour lors de chaque démarrage de votre application.

###### Navigation rapide
* [Retour au sommaire des API](./README.md)
* [Retour à l'index](../README.md)