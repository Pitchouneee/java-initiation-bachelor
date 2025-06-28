# 🧙‍♂️ Projet – Mini RPG : Combat au tour par tour

## 🎯 Objectifs du projet

Ce projet final te permet d’appliquer des notions avancées de la POO :

- Création de **classes abstraites et héritées**
- **Polymorphisme** via des méthodes redéfinies
- Gestion d’une **boucle de jeu interactive**
- Manipulation d’attributs dynamiques (points de vie, attaques)

Tu vas créer un petit jeu de combat au tour par tour entre deux personnages ayant des capacités différentes.


## 🧩 Fonctionnalités attendues

- Créer une classe **abstraite** `Personnage` avec :
  - `String nom`
  - `int vie`
  - Méthode `attaquer(Personnage cible)` (abstraite ou redéfinissable)
- Créer deux **sous-classes** :
  - `Guerrier` (fort, attaque physique)
  - `Magicien` (plus fragile mais puissant, peut infliger des coups spéciaux)
- Mettre en place un **système de combat** dans la console :
  - Tour par tour : chaque personnage attaque l’autre
  - La vie diminue à chaque coup
  - Affichage de l’état après chaque attaque
- Le jeu s’arrête quand un personnage n’a plus de points de vie

## ✅ Exécution attendue

```yaml
🧙 Bienvenue dans le Mini-RPG Java 🗡️

Guerrier : Ragnar [💖 100 HP]
Magicien : Merlin [💖 80 HP]

-- Tour 1 --
Ragnar attaque avec son épée !
Merlin perd 20 points. [💖 60 HP]

Merlin lance une boule de feu !
Ragnar perd 30 points. [💖 70 HP]

-- Tour 2 --
...

🎉 Victoire de Merlin !
```

## 🧠 Bonus

- Ajouter des **compétences spéciales** (coup critique, soin, défense…)
- Utiliser une interface `Competence` pour spécialiser certaines attaques
- Ajouter des objets consommables (ex : potions de vie)
- Système d’**expérience et niveaux**

🗂️ Structure libre

Tu es libre d’organiser tes classes dans plusieurs fichiers (`Personnage.java`, `Guerrier.java`, `Magicien.java`, etc.).

Le but est de montrer que tu sais structurer un programme orienté objet cohérent et réutilisable.

## 🧩 Besoin d’un coup de pouce ?

🛡️ C’est ton combat ! Mais si ton magicien n’incante plus rien, appelle ton intervenant pour une potion de clarté ✨

## 📤 Consignes de rendu

Toutes les consignes détaillées pour le rendu final (GitHub, README, noms des membres, etc.) sont disponibles ici :

📄 [projets/consignes.md](consignes.md)

> Assure-toi de bien les lire avant de remettre ton projet !