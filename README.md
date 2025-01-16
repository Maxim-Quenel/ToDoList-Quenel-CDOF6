# Gestionnaire de Tâches (CLI)

##-> Description
Ce projet est un gestionnaire de tâches simple basé sur une interface en ligne de commande (CLI). Il permet d'ajouter, de visualiser, de marquer comme terminées ou de supprimer des tâches, avec une sauvegarde automatique dans un fichier JSON.

##-> Fonctionnalités
- **Ajout de tâches** : Saisissez le nom, la description et la date d'échéance d'une tâche.
- **Affichage des tâches** : Liste toutes les tâches avec leur état ("En cours" ou "Terminée").
- **Marquage comme terminée** : Change l'état d'une tâche en "Terminée".
- **Suppression de tâches** : Supprime une tâche spécifique de la liste.
- **Sauvegarde automatique** : Les tâches sont sauvegardées dans un fichier `tasks.json` lors de la fermeture du programme et chargées automatiquement au démarrage.

##-> Prérequis
- Python 3.x

##-> Installation
1. Clonez le dépôt ou téléchargez le fichier Python.
2. Assurez-vous que Python est installé sur votre machine.
3. Aucun module externe n'est requis.

##-> Utilisation
1. Lancez le script avec la commande :
   ```bash
   python script.py
   ```
2. Suivez les instructions affichées dans le menu pour gérer vos tâches.

##-> Menu Principal
- `1` : Ajouter une tâche
- `2` : Afficher les tâches
- `3` : Marquer une tâche comme terminée
- `4` : Supprimer une tâche
- `5` : Quitter (avec sauvegarde automatique)

##-> Exemple d'utilisation
### Ajouter une tâche
- Saisissez un nom de tâche, une description et une date d'échéance au format `YYYY-MM-DD`.

### Afficher les tâches
- Affiche une liste de toutes les tâches avec leur état :
  ```
  1. [En cours] Faire les courses - Acheter des fruits et légumes (Échéance : 2025-01-15)
  2. [Terminée] Appeler Jean - Planifier une réunion (Échéance : 2025-01-10)
  ```

### Marquer une tâche comme terminée
- Entrez le numéro de la tâche à marquer comme terminée.

### Supprimer une tâche
- Entrez le numéro de la tâche à supprimer.

##-> Fichier JSON
Les tâches sont sauvegardées dans un fichier `tasks.json` au format suivant :
```json
[
    {
        "name": "Faire les courses",
        "description": "Acheter des fruits et légumes",
        "due_date": "2025-01-15",
        "completed": false
    },
    {
        "name": "Appeler Jean",
        "description": "Planifier une réunion",
        "due_date": "2025-01-10",
        "completed": true
    }
]
```

##-> Améliorations futures
- Gestion des priorités pour les tâches.
- Notifications pour les échéances imminentes.
- Interface graphique (GUI) pour une meilleure expérience utilisateur.

##-> Auteur
Tristan

##-> Licence
Ce projet est sous licence MIT. Vous êtes libre de l'utiliser, de le modifier et de le distribuer.
