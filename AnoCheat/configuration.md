# Configuration
L'API vous permet d'interagir avec la configuration des modules, afin d'éviter tout désagrément il est déconseillé de modifier la 
configuration des autres modules. Néanmoins vous pouvez vous baser sur les paramètres d'un module ou d'une dépendance si nécessaire.

##### Ecrire / modifier la configuration
```Javascript
AC_configWrite('moduleName', {'status':'enabled', 'msg':'Hello world!'});
```

##### Lire la configuration
```Javascript
AC_configRead('moduleName');
```

###### Bon à savoir
`AC_configWrite()` n'écrit que les clés renseignées et ne touche pas les autres valeurs. Pour effacer une clé remplacez sa valeur par `undefined`

###### Navigation rapide
[Retour au sommaire des Anocheat](./readme.md)
[Retour à l'index]('../readme.md)