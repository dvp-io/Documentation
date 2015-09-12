#Menus
L'API interne propose une approche simplifiée et unifiée pour créer des menus et boutons. Ces derniers sont nécessaires pour 
permettre un accès rapide à une interface de configuration, changer l'état d'une option, executer une requête ou toute autre 
fonctionalité.

##### Création d'un menu
```Javascript
AC_addMenu('Mon premier menu', 'Ceci est un menu \o/', callback);
```

##### Création d'un bouton avec interaction
```Javascript
AC_addButton('Mon premier bouton', callback);
```

###### Bon à savoir
Vous pouvez interagir facilement avec le menu et bouton :

```Javascript
AC_addButton('Mon premier bouton', function() {
  this.style.textDecoration = 'line-through';
});
```

Au clic sur le bouton son texte sera barré
![](http://media.dvp.io/anocheat/preview/premier_bouton.png)

###### Navigation rapide
* [Retour au sommaire des AnoCheat](./readme.md)
* [Retour à l'index]('../readme.md)