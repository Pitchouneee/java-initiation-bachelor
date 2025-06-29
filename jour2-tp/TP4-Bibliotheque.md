# TP4 – 📚 Gestionnaire de bibliothèque

**Objectifs :** Découvrir la POO : création de classes, objets, listes et interaction

## 🎓 Cours lié : Classes, objets, constructeurs et ArrayList

Ce TP t’initie à la **programmation orientée objet (POO)**, pilier fondamental de Java. Tu vas apprendre à :

- Définir des **classes** pour représenter des entités (ici, des livres 📖)
- Créer des **objets** à partir de ces classes
- Stocker ces objets dans une **collection dynamique** (`ArrayList`)
- Manipuler tout cela à travers un menu interactif

📚 Pour aller plus loin :

- [Documentation `ArrayList`](https://docs.oracle.com/en/java/javase/21/docs/api/java.base/java/util/ArrayList.html)
- [Syntaxe des classes – Oracle](https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html)

### 🧱 Classe et objet : la base de la POO

Une classe est un **plan de construction**. Un objet est une **instance** de cette classe :

```java
public class Livre {
    String titre;
    String auteur;
    String isbn;
}
```

Créer un objet :

```java
Livre monLivre = new Livre();
monLivre.titre = "1984";
monLivre.auteur = "George Orwell";
```

### 🛠️ Constructeur

Un *constructeur* initialise un objet avec des valeurs :

```java
public class Livre {
    String titre, auteur, isbn;

    public Livre(String titre, String auteur, String isbn) {
        this.titre = titre;
        this.auteur = auteur;
        this.isbn = isbn;
    }
}
```

Et pour l’utiliser :

```java
Livre livre = new Livre("Dune", "Frank Herbert", "978-0441013593");
```

### 📚 Gérer une collection avec `ArrayList`

`ArrayList` permet de stocker plusieurs objets dynamiquement :

```java
import java.util.ArrayList;

ArrayList<Livre> bibliotheque = new ArrayList<>();

bibliotheque.add(l);            // ajouter un livre
bibliotheque.remove(0);         // supprimer le livre à l’index 0
bibliotheque.get(0);            // accéder au premier livre
bibliotheque.size();            // nombre d’éléments
```

> [!NOTE]
> On peut aussi parcourir la liste avec une boucle for pour afficher les livres

## 🎯 Objectifs du TP

Tu vas coder un gestionnaire de bibliothèque en ligne de commande avec les fonctionnalités suivantes :

- Créer une classe `Livre` avec :
    - titre (String)
    - auteur (String)
    - isbn (String)
-  Afficher un menu interactif
    - Ajouter un livre
    - Lister tous les livres
    - Rechercher un livre par un titre
    - Supprimer un livre
- Utiliser une `ArrayList<Livre>` pour stocker les livres

## ✅ Exécution attendue

```yaml
📚 Bienvenue dans votre bibliothèque

1 - Ajouter un livre
2 - Lister les livres
3 - Rechercher un livre par titre
4 - Supprimer un livre
5 - Quitter

1
Titre : Dune
Auteur : Frank Herbert
ISBN : 978-0441013593

[Livre ajouté ✅]

2
📘 Dune – Frank Herbert – 978-0441013593

3
Titre à rechercher : dune
📘 Livre trouvé : Dune – Frank Herbert – 978-0441013593

4
Quel livre supprimer ? (titre exact) : Dune
[Livre supprimé ✅]

5
👋 À bientôt !
```

## 🧠 Bonus

- Sauvegarder les livres dans un fichier `.txt` (avec `FileWriter`)
- Trier les livres par titre (`Collections.sort`)
- Rendre la recherche insensible à la casse (`toLowerCase()`)

## 🧩 Besoin d’un coup de pouce ?

🧱 Si tu te heurtes à un mur, appelle le prof avant de le défoncer !

📘 **Pour aller plus loin :**

- 📝 [TP6 – Carnet de notes](../bonus/TP6-Carnet-de-notes.md) : découvre comment sauvegarder ta bibliothèque dans un fichier texte
- 📦 [TP7 – Structurer son projet Java](../bonus/TP7-Packages-et-organisation.md) : apprends à organiser ton code comme un vrai dev