dans ce fichier vous trouverez les commande git necessaire pour utiliser, travailler et partager votre travail sur le projet avec les autre. revenez y quand vous avez besoin et/ou demandez ou parlez au autre si vous doutez pour evitez tout bugs ou accidents.

# Mémo des commandes Git

## 1. Initialisation du projet (Une seule fois)

| Commande | Explication |
| :--- | :--- |
| `git clone <url>` | Télécharge un repository GitHub existant (et son `.gitignore`) directement sur le PC. |
| `git init` | *(Alternative)* Transforme un dossier local classique en dépôt Git. |
| `git remote add origin <url>` | Lie un dépôt local fraîchement initialisé à sa destination sur GitHub. |
| `git branch -M main` | Renomme la branche principale par défaut en `main`. |

## 2. Synchronisation (Au début de chaque session)

| Commande | Explication |
| :--- | :--- |
| `git pull origin main` | Télécharge et intègre le nouveau code poussé par les collègues. Étape obligatoire avant de coder pour éviter les conflits. |

## 3. Le travail isolé (Gestion des branches)

| Commande | Explication |
| :--- | :--- |
| `git switch -c <nom-branche>` | Crée une nouvelle branche de brouillon isolée et bascule dessus instantanément. |
| `git switch main` | Quitte le brouillon pour revenir sur la branche principale `main`. |
| `git branch -d <nom-branche>` | Supprime une branche locale une fois qu'elle a été fusionnée. |

## 4. Sauvegarde et Envoi (Le cycle quotidien)

| Commande | Explication |
| :--- | :--- |
| `git status` | Affiche l'état en temps réel (fichiers modifiés, préparés, ou conflits en cours). |
| `git add .` | Sélectionne tous les fichiers modifiés et les place dans la zone de préparation (remplit le carton). |
| `git commit -m "Message"` | Valide la préparation et l'enregistre définitivement dans l'historique local (ferme le carton et l'étiquette). |
| `git push` | Envoie toutes les sauvegardes locales vers GitHub. |
| `git push -u origin <nom-branche>` | À utiliser **uniquement lors du premier envoi** d'une nouvelle branche pour créer son équivalent sur GitHub. |

## 5. La fusion (Intégration du travail terminé)

| Commande | Explication |
| :--- | :--- |
| `git merge <nom-branche>` | Aspire le contenu de la branche spécifiée pour l'intégrer dans la branche actuelle (généralement `main`). |
