# Gestion des styles

Le script vous permet de définir un style autre que celui du chat, cela vous permet de créer vos propres designs et de les proposer aux autres membres en effectuant un push sur le repo du projet.

Pour que votre style soit accepté il doit respecter les conditions suivantes :

- Ne masquer aucun élément au sein des menus, conversation, liste des membres et boites de dialogues
- Prendre en charge l'intégralité du chat (menus, conversations, listes, boites de dialogues, AnoCheat, GeckoScript)
- Le CSS non minifié et toutes les images utilisées doivent êtres envoyées sur le repo du projet en respectant l'arborescence
- Les images ajoutées doivent êtres appelées depuis le repo du projet, GitHub fournissant une haute disponibilité

En cas de retours négatifs vous serez notifiés, vous devez avoir une certaine réactivité pour corriger les problèmes visuels afin de garantir l'expérience des utilisateurs.

## GS_addStyle
La méthode GS_addStyle vous permet d'ajouter facilement un design à la sélection. Les paramètres sont:

- **name :** nom du style, ce nom sert de classe parente
- **css :** Le code CSS de votre style

```Javascript
GS_addStyle('name','css');
```

## Mono
Le style mono permet de conserver une certaine discrétion, le chat passe intégralement en noir sur fond blanc.

## Console
Le style console est l'inverse du style mono, il passe l'intégralité du chat en blanc sur fond noir
