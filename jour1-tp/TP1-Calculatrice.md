# TP1 – 🧮 Calculatrice CLI

**Objectifs :** Manipuler les entrées clavier, les conditions et les opérations mathématiques de base.

## 🎓 Cours lié : Les bases de Java (variables, types, opérateurs, `Scanner`)

Ce premier TP est l'occasion parfaite pour découvrir les **fondations du langage Java**. Tu apprendras à :

- Déclarer et manipuler des **variables**
- Effectuer des **opérations arithmétiques**
- Lire des données saisies par l’utilisateur avec `Scanner`
- Utiliser une **structure conditionnelle** (`switch` ou `if-else`)

### 🔢 Les types de variables

Java est un langage **fortement typé**. Chaque variable doit avoir un type :

```java
int age = 25;
double temperature = 36.5;
String nom = "Alice";
```

### 🧮 Les opérateurs

Voici les opérations de base que tu peux faire avec Java :

```java
int a = 4 + 2;    // addition
int b = 6 - 3;    // soustraction
int c = 5 * 2;    // multiplication
int d = 10 / 2;   // division entière
```
> [!WARNING]  
> Attention : 10 / 3 avec deux entiers retourne 3, pas 3.33.

### 🎙️ Lire l’entrée utilisateur avec Scanner

Java permet de lire ce que l’utilisateur tape grâce à la classe `Scanner` :

```java
Scanner scanner = new Scanner(System.in);
System.out.print("Entrez un nombre : ");
int x = scanner.nextInt();
```

> [!NOTE]
> 📌 Remarque : pour lire une ligne complète après un `nextInt()` ou `nextDouble()`, pense à appeler `scanner.nextLine()` pour consommer le saut de ligne restant.

## 🎯 Objectifs du TP

Créer une petite calculatrice qui fonctionne dans le terminal :

- Demander deux nombres à l'utilisateur
- Demander une opération (`+`, `-`, `*`, `/`)
- Afficher le résultat
- Gérer la division par zéro

## ✅ Exécution attendue

```java
Entrez le premier nombre : 8
Entrez l'opération (+, -, *, /) : *
Entrez le deuxième nombre : 3
Résultat : 24
```

> 💡 Astuce : un petit switch et ça repart ! (Parfait pour tester le type d'opération à faire)

## 🧠 Bonus

- Refaire un calcul tant que l’utilisateur veut
- Supporter les décimales avec double au lieu de int