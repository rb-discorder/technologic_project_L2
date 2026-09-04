# Aide-Mémoire : Commandes Terminal et Unix

## 1. Raccourcis & Édition
| Commande / Raccourci | Description |
| :--- | :--- |
| `Tab` | Complétion automatique d'une commande ou d'un nom de fichier. |
| `Flèche Haut` / `Flèche Bas` | Naviguer dans l'historique des commandes (précédentes / récentes). |
| `Ctrl + r` | Rechercher rapidement une ancienne commande dans l'historique. |
| `Ctrl + c` | Interrompre l'exécution de la commande en cours. |
| `Ctrl + Shift + c` | Copier le texte sélectionné dans un terminal (Linux). |
| `Ctrl + Shift + v` | Coller le texte dans un terminal (Linux). |
| `Clic milieu` | Coller rapidement un texte préalablement sélectionné à la souris. |

## 2. Historique & Infos
| Commande | Description |
| :--- | :--- |
| `history` | Afficher l'historique complet des commandes tapées et leur numéro. |
| `!42` | Relancer directement la commande correspondant au numéro 42 de l'historique. |
| `whoami` | Afficher l'identifiant de l'utilisateur actuellement connecté. |
| `date` | Afficher la date et l'heure du système. |
| `cal` | Afficher un calendrier (ex: `cal 2005` affiche l'année 2005). |
| `file <fichier>` | Déterminer le type réel d'un fichier, indépendamment de son extension. |

## 3. Système de fichiers, Navigation & Base
| Commande / Symbole | Description |
| :--- | :--- |
| `/` | Répertoire racine de l'arborescence du système (chemin absolu). |
| `.` | Répertoire courant (celui dans lequel on se trouve). |
| `..` | Répertoire parent (permet de remonter d'un dossier dans l'arborescence). |
| `~` | Raccourci désignant le répertoire personnel de l'utilisateur (home directory). |
| `$HOME` | Variable d'environnement pointant vers le répertoire personnel (`echo $HOME`). |
| `pwd` | Afficher le chemin absolu du répertoire dans lequel on se trouve actuellement. |
| `cd` | Changer de répertoire courant (ex: `cd ..` pour remonter). |
| `ls` | Lister le contenu d'un répertoire. |
| `mkdir` | Créer un nouveau répertoire. |
| `rm` | Supprimer des fichiers ou des répertoires. |
| `cp` | Copier un fichier ou un répertoire. |
| `mv` | Déplacer ou renommer un fichier ou un répertoire. |

## 4. Commandes Avancées
| Commande | Description |
| :--- | :--- |
| `chmod` | Modifier les droits d'accès (lecture, écriture, exécution) d'un fichier. |
| `grep` | Rechercher une chaîne de caractères spécifique dans un ou plusieurs fichiers. |
| `find` | Rechercher des fichiers dans l'arborescence selon divers critères. |
| `tar` | Regrouper plusieurs fichiers dans une archive (et/ou les compresser). |
| `>`, `>>`, `<` | Rediriger la sortie standard vers un fichier (écraser ou ajouter) ou l'entrée standard. |
| `\|` (Tube) | Connecter la sortie d'une commande à l'entrée d'une autre. |

## 5. Explication des Options Courantes

Les options (ou drapeaux) modifient le comportement des commandes. Elles se combinent souvent (ex: `ls -lah`).

### Options pour lister les fichiers (`ls`)
| Option | Nom | Description |
| :--- | :--- | :--- |
| `-l` | Long format | Liste détaillée (droits d'accès, propriétaire, taille, date de modification). |
| `-a` | All | Affiche **tous** les fichiers, y compris les fichiers cachés (commençant par `.`). |
| `-h` | Human readable | Affiche la taille en format lisible (Ko, Mo) au lieu d'octets bruts (souvent `ls -lh`). |

### Options pour manipuler (`cp` / `rm`)
| Option | Nom | Description |
| :--- | :--- | :--- |
| `-r` (ou `-R`) | Récursif | **Indispensable pour les dossiers.** S'applique au dossier et à tout son contenu. |
| `-f` | Force | Force l'action sans demander de confirmation et sans afficher d'erreur si inexistant. |
| `-rf` | Récursif + Force | **⚠️ Attention.** Supprime un dossier et son contenu de force, sans confirmation (`rm -rf`). |
| `-i` | Interactif | Demande une confirmation (y/n) avant d'écraser ou supprimer chaque fichier. |

### Autres options utiles
| Commande + Option | Description |
| :--- | :--- |
| `mkdir -p` | **P**arents. Crée une arborescence complète d'un coup (ex: `mkdir -p A/B/C`). |
| `commande --help` | Affiche l'aide et les options disponibles pour la commande. |
| `man commande` | Ouvre le manuel complet de la commande. Appuyez sur `q` pour quitter. |
