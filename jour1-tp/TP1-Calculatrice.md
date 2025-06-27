# TP1 – 🧮 Calculatrice CLI
**Objectifs :** Manipuler les entrées clavier, les conditions et les opérations mathématiques de base.

## 🎓 Cours lié : Les bases de Java (variables, types, opérateurs, `Scanner`)
Avant de te lancer dans ce TP, voici quelques notions utiles :

### 🔢 Les types de variables
```java
int age = 25;
double temperature = 36.5;
String nom = "Alice";
```

### 🧮 Les opérateurs
```java
int a = 4 + 2;    // addition
int b = 6 - 3;    // soustraction
int c = 5 * 2;    // multiplication
int d = 10 / 2;   // division entière
```

### 🎙️ Lire l’entrée utilisateur avec Scanner
```java
Scanner scanner = new Scanner(System.in);
System.out.print("Entrez un nombre : ");
int x = scanner.nextInt();
```

## 🎯 Objectifs du TP
Créer une petite calculatrice qui fonctionne dans le terminal :
- Demander deux nombres à l'utilisateur
- Demander une opération (`+`, `-`, `*`, `/`)
- Afficher le résultat
- Gérer la division par zéro

## ✅ Exécution attendue
```java
Nombre 1 : 8
Opération (+, -, *, /) : *
Nombre 2 : 3
Résultat : 24
```

## 🧠 Bonus
- Refaire un calcul tant que l’utilisateur veut
- Supporter les décimales avec double au lieu de int