# Simulation d'un écosystème Moutons-Herbe (NetLogo)

Ce projet est un modèle multi-agents réalisé sous **NetLogo** simulant l'interaction entre des agents mobiles (tortues/moutons) et leur environnement (herbe).

## Fonctionnement de la simulation

* **L'environnement (Patches) :** La grille est composée de parcelles d'herbe (`green`) et de terre (`brown`). Lorsqu'une parcelle d'herbe est mangée, elle devient marron et repousse automatiquement après un délai défini.
* **Les agents (Turtles) :** Les tortues se déplacent aléatoirement sur la grille et perdent de l'énergie à chaque pas. Lorsqu'elles rencontrent une parcelle verte, elles la mangent (gagnent de l'énergie) et tournent de 90 degrés. Si leur énergie atteint `0`, elles disparaissent.

## Paramètres de l'interface (Inputs)

Avant de lancer la simulation, l'utilisateur peut configurer les valeurs suivantes sur l'interface :

| Paramètre | Description | Exemple de valeur |
| :--- | :--- | :--- |
| **`Densite_herbe`** | Pourcentage initial de parcelles vertes au démarrage (0 à 100). | `40` |
| **`Temps_repousse_herbe`** | Nombre de *ticks* nécessaires pour qu'une parcelle marron redevienne verte. | `15` |
| **`nb_turtles`** | Nombre de tortues créées lors de l'initialisation. | `20` |
| **`energie_initiale_turtle`** | Niveau d'énergie de départ de chaque tortue. | `10` |

## Comment exécuter le modèle

1. Ouvrir le fichier `.nlogo` avec le logiciel **NetLogo**.
2. Renseigner les valeurs souhaitées dans les champs **Input** et valider avec la touche **Entrée**.
3. Cliquer sur le bouton **`setup`** pour initialiser le terrain et les tortues.
4. Cliquer sur le bouton **`go`** (en mode *Forever*) pour démarrer la simulation.
