# Règles de gestion Git du projet

Ces règles s'appliquent automatiquement à l'assistant et aux contributeurs de ce projet.

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
  ```bash
  git push
  ```

> [!NOTE]
> Pour que la commande `git push` fonctionne, un dépôt distant (`origin`) doit être configuré (par exemple : `git remote add origin <url_du_depot>` puis `git push -u origin master`).
