# Notifications
Vous pouvez notifier un utilisateur de manière très simple. Selon la configuration choisie par l'utilisateur il recevra une 
notification visuelle, sonore et/ou textuelle. Les notifications sont adaptées automatiquement par l'API, vous n'avez qu'à 
envoyer votre message initial.

Pour notifier l'utilisateur vous pouvez utiliser l'événement `user:notify` ou la méthode `AC_notify`, le comportement est exactement le même.

Le standard établi pour les notifications limite la taille des messages à 140 caractères.

##### Notifier un utilisateur
```Javascript
AC_emit('user:notify', 'Hello world!');
```

```Javascript
AC_notify('Hello world!');
```

###### Navigation rapide
* [Retour au sommaire des Anocheat](./readme.md)
* [Retour à l'index]('../readme.md)
