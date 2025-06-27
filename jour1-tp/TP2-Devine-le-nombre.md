# TP2 – 🎲 Devine le nombre !
**Objectifs :** Utiliser les boucles et générer un nombre aléatoire.

## 🎓 Cours lié : Boucles et nombres aléatoires
Avant de te lancer dans ce TP, voici quelques notions utiles :

### 🔁 Boucle `while`
```java
int x = 0;
while (x < 5) {
    System.out.println("x vaut : " + x);
    x++;
}
```

### 🔁 Boucle `do-while`
```java
int x;
do {
    System.out.print("Entrez un nombre > 0 : ");
    x = scanner.nextInt();
} while (x <= 0);
```

### 🎲 Générer un nombre aléatoire
```java
import java.util.Random;

Random rand = new Random();
int secret = rand.nextInt(100) + 1; // entre 1 et 100
```

## 🎯 Objectifs du TP
- Le programme choisit un nombre aléatoire entre 1 et 100
- L’utilisateur doit deviner ce nombre
- Indiquer “plus” ou “moins” jusqu’à la bonne réponse
- Compter le nombre d’essais

## ✅ Exécution attendue
```java
Nombre 1 : 8
Opération (+, -, *, /) : *
Nombre 2 : 3
Résultat : 24
```

## 🧠 Bonus
- Ajouter un système de scores ou rejouer
