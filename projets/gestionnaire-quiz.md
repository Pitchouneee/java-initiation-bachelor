# ❓ Projet – Gestionnaire de Quiz

## 🎯 Objectifs du projet

Ce projet final met en pratique tout ce que tu as vu :

- La **programmation orientée objet**
- La **manipulation de listes**
- L’interaction utilisateur en ligne de commande
- La gestion d’un **score dynamique**

Tu vas construire un petit jeu-questionnaire dans lequel l’utilisateur répond à des QCM, reçoit une correction et un score.

## 🧩 Fonctionnalités attendues

- Créer une classe `Question` contenant :
  - Un intitulé
  - Trois choix possibles
  - L’indice ou lettre de la bonne réponse
- Charger une liste de questions depuis le fichier fourni :  
  📄 [`projets/questions.txt`](questions.txt)
- Afficher chaque question dans la console avec les choix a), b), c)
- Demander à l’utilisateur sa réponse
- Indiquer s’il a eu bon ou faux
- Afficher un **score final**

## ✅ Exécution attendue

```yaml
Bienvenue dans le Quiz Java 🎓

Question 1/5 :
Quelle est la méthode principale pour exécuter un programme Java ?
a) start()
b) main(String[] args)
c) launch()

b
✔️ Bonne réponse !

...

Résultat final : 4/5 🎉
```

## 🧠 Bonus

- Ajouter un **chronomètre** pour mesurer la durée totale (avec `System.currentTimeMillis()`)
- Sauvegarder le **score dans un fichier texte**
- Permettre à l’utilisateur de **rejouer** plusieurs fois
- Introduire des **niveaux** selon le score

## 🗂️ Données fournies

Un fichier `questions.txt` est disponible dans le dossier `projets/` pour éviter de devoir écrire les questions manuellement.

```yaml
Format :
Question 1 ?
a) réponse A
b) réponse B
c) réponse C
réponse: b
```

> ✅ À toi d’écrire le code qui lit ce fichier, extrait les blocs, et les transforme en objets `Question`.

## 🧩 Besoin d’un coup de pouce ?

🧠 C’est un projet final, alors cherche bien par toi-même. Mais si tu bloques vraiment, demande un petit indice 😉

## 📤 Consignes de rendu

Toutes les consignes détaillées pour le rendu final (GitHub, README, noms des membres, etc.) sont disponibles ici :

📄 [projets/consignes.md](consignes.md)

> Assure-toi de bien les lire avant de remettre ton projet !