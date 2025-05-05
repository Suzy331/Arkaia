# Arkaia - Bibliothèque de Gestion de Livres

**Arkaia** est un projet C qui implémente une bibliothèque de gestion de livres. Le programme permet de gérer les utilisateurs, les auteurs, les livres, et les actions d'emprunt et de retour. L’objectif est de créer une application de gestion de bibliothèque simple, avec des fonctionnalités de sauvegarde et de chargement des données depuis des fichiers.

## Fonctionnalités

- **Gestion des utilisateurs** : Ajouter, modifier et lister les utilisateurs.
- **Gestion des auteurs** : Ajouter, modifier et lister les auteurs.
- **Gestion des livres** : Ajouter, modifier, lister les livres et associer un livre à un auteur.
- **Actions** : Enregistrer les actions d'emprunt et de retour de livres.
- **Sauvegarde et chargement des données** : Les données (utilisateurs, auteurs, livres, actions) sont stockées dans des fichiers texte.

## Structure du projet

```
├── bin/               # Contient les fichiers binaires générés par la compilation
├── build/             # Répertoire temporaire de compilation
├── data/              # Contient les fichiers de données (utilisateurs, livres, actions)
│   ├── actions.txt    # Liste des actions effectuées sur les livres
│   ├── auteurs.txt    # Liste des auteurs
│   ├── books.txt      # Liste des livres
│   └── users.txt      # Liste des utilisateurs
├── include/           # Contient les fichiers d'en-tête (.h)
│   ├── user.h         # Déclarations liées aux utilisateurs
│   ├── auteur.h       # Déclarations liées aux auteurs
│   ├── book.h         # Déclarations liées aux livres
│   └── action.h       # Déclarations liées aux actions
├── src/               # Contient les fichiers source (.c)
│   ├── user.c         # Code pour gérer les utilisateurs
│   ├── auteur.c       # Code pour gérer les auteurs
│   ├── book.c         # Code pour gérer les livres
│   └── action.c       # Code pour gérer les actions (emprunts et retours)
├── tests/             # Contient les tests pour chaque module
│   └── test_user.c    # Test des fonctionnalités liées aux utilisateurs
├── Makefile           # Script de compilation
└── README.md          # Documentation du projet
```

## Compilation

Pour compiler le projet, utilisez la commande suivante :

```bash
make
```

## Tests

Des tests unitaires sont fournis pour tester les principales fonctionnalités du programme. Vous pouvez les exécuter avec la commande suivante :

```bash
make test
```

## Utilisation

1. **Charger les livres** depuis le fichier `data/books.txt` avec la fonction `charger_books()`.
2. **Ajouter un livre** avec la fonction `ajouter_book()`.
3. **Afficher la liste des livres** avec `afficher_books()`.
4. **Enregistrer et charger les actions** d'emprunt et de retour des livres.

## Contribuer

Si vous souhaitez contribuer à ce projet, vous pouvez ouvrir une **pull request** en suivant les étapes ci-dessous :

1. Fork le projet
2. Créez une branche (`git checkout -b feature/nom-de-la-feature`)
3. Committez vos modifications (`git commit -am 'Ajout de nouvelles fonctionnalités'`)
4. Poussez la branche (`git push origin feature/nom-de-la-feature`)
5. Ouvrez une pull request

## License

Ce projet est sous la licence MIT. Voir le fichier `LICENSE` pour plus de détails.

