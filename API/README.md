# Les API

Toutes nos API web sont disponibles via [https://api.dvp.io](https://api.dvp.io) et sont totalement gratuites. Néanmoins pour pouvoir en bénéficier vous devez être membre de la 
[communauté développez](http://www.developpez.net). Actuellement seul le chat dispose d'un mécanique permettant de vous identifier en tant que membre sans renseigner vos identifiants, de ce fait les API
ont actuellement une portée limitée.

Nous espérons que cela changera dans un avenir proche afin de pouvoir vous fournir toujours plus d'outils, gratuits, de qualité et sans publicité.

## Structure des données reçues

Quelque soit l'API les données sont toujours structurées de la même manière:
```Javascript
{
  data: {"contiens les données de l'API"},
  api:  {"contiens les infos de l'API"},
  core: {"contiens les infos du gestionnaire d'API"}
}
```

En cas d'erreur un message est retourné, l'ID indique d'où proviens l'erreur, le message permet de résoudre le problème.
```Javascript
{
  error: { id: 'string', msg: 'string' }
}
```

En cas de succès un message est retourné en l'absence de données.
```
{
  success: { msg: 'string' }
}
```

## Liste des API

* [Alias](./alias.md)
> Enregistrez facilement des paires clé/valeur et réutilisez-les dans vos applications

* [Amis](./amis.md)
> Permet de récupérer la liste d'amis développez d'un membre

* [Cloud](./cloud.md)

* [Feed](./feed.md)
> Cette API génère un flux vous permettant de vous abonner à un ou plusieurs types de contenus (blog, articles, actualités) et à différentes catégories (PHP, JS, C, 3D ect...)

* [Search](./search.md)
> Effectuez des recherches par thématique

* [Smileys](./smileys.md)
> Obtenez plus de 300 smileys disponibles pour tous et intégrez les facilement à votre application


###### Navigation rapide
* [Retour à l'index](../README.md)