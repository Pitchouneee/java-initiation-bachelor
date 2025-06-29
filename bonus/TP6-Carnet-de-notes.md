# TP6 – 📝 Carnet de notes

**Objectifs :** Lire et écrire des données dans un fichier texte, manipuler des listes d’objets

## 🎓 Cours lié :

- Fichiers avec `Scanner` et `FileWriter`
- Collections (`ArrayList`)
- Classes Java simples

## 🎯 Objectifs du TP

Créer un carnet de notes dans la console qui :

- Charge une liste d’élèves depuis un fichier `.txt`
- Affiche tous les élèves et leur moyenne
- Permet d’ajouter un nouvel élève
- Enregistre les modifications dans le fichier

## 📄 Fichier source : [`notes.txt`](notes.txt)

```txt
Alice;15.5
Bob;12.0
Charlie;17.25
```

Chaque ligne contient un nom suivi d’une moyenne (séparés par `;`)

## ✏️ Étapes du TP

1. Créer une classe `Eleve` avec `String nom` et `double moyenne`
2. Lire le fichier `notes.txt` ligne par ligne
3. Utiliser `split(";")` pour séparer nom et note
4. Ajouter chaque élève à une `ArrayList<Eleve>`
5. Afficher la liste complète
6. Proposer d’en ajouter un nouveau via la console
7. Sauvegarder la liste complète dans le fichier

## ✅ Exécution attendue

```yaml
📒 Liste des élèves :

- Alice : 15.5
- Bob : 12.0
- Charlie : 17.25

Ajouter un nouvel élève ? (o/n)
> o

Nom : Zoé
Moyenne : 13.75

✅ Élève ajouté et sauvegardé !
```

## 🧠 Bonus

- Calculer la moyenne générale de la classe
- Trier par note décroissante
- Gérer les erreurs de format dans le fichier