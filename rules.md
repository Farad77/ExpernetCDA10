# Règles de gestion Git du projet

Ces règles s'appliquent automatiquement à l'assistant et aux contributeurs de ce projet.

---

## Mode de fonctionnement actuel : Local uniquement
> [!NOTE]
> Aucun dépôt distant (`remote`) n'est configuré pour le moment. Toutes les opérations restent en local (`git add` et `git commit`). Les commandes `git push` sont mises en attente jusqu'à l'ajout explicite d'un `remote`.

---

## 1. Modifications ou ajouts en cours de développement
À chaque modification ou ajout de code ou de fichier :
- **Ajout des modifications** :
  ```bash
  git add .
  ```
- **Création du commit** avec un message descriptif :
  ```bash
  git commit -m "feat/fix/chore: description claire des modifications"
  ```

---

## 2. Finalisation d'un fichier
Dès qu'un fichier est complété / finalisé :
- **Ajout et commit des derniers changements** :
  ```bash
  git add .
  git commit -m "complete: finalisation du fichier <nom_du_fichier>"
  ```
- **Envoi sur le dépôt distant (Push)** :
  *(Uniquement lorsqu'un dépôt distant aura été configuré)*
  ```bash
  git push
  ```
