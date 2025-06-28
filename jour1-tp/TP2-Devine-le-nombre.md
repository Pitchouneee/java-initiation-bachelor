# TP2 – 🎲 Devine le nombre !

**Objectifs :** Utiliser les boucles et générer un nombre aléatoire

## 🎓 Cours lié : Boucles et nombres aléatoires

Dans ce TP, tu vas découvrir comment **répéter une action tant qu'une condition n'est pas remplie**, et comment **faire choisir un nombre par l’ordinateur**.

C’est l’occasion parfaite pour :
- Te familiariser avec les **boucles conditionnelles**
- Créer un **jeu interactif simple et addictif**
- Apprendre à utiliser `Random` pour le côté imprévisible 🎲

### 🔁 Boucle `while`

Une boucle `while` permet de **répéter un bloc de code tant qu'une condition est vraie**. Exemple :

```java
int x = 0;
while (x < 5) {
    System.out.println("x vaut : " + x);
    x++;
}
```

### 🔁 Boucle `do-while`

Contrairement à `while`, la boucle `do-while` **exécute le bloc au moins une fois**, même si la condition est fausse dès le début.

```java
int x;
do {
    System.out.print("Entrez un nombre > 0 : ");
    x = scanner.nextInt();
} while (x <= 0);
```

### 🎲 Générer un nombre aléatoire

Java propose la classe `Random` pour obtenir des valeurs pseudo-aléatoires :

```java
import java.util.Random;

Random rand = new Random();
int secret = rand.nextInt(100) + 1; // entre 1 et 100
```

> [!NOTE]  
> nextInt(100) donne un nombre entre 0 et 99, donc on ajoute +1 pour avoir [1, 100].

## 🎯 Objectifs du TP

Créer un programme interactif dans lequel :

- Le programme choisit un nombre aléatoire entre 1 et 100
- L’utilisateur doit deviner ce nombre
- Indiquer “plus” ou “moins” jusqu’à la bonne réponse
- Compter le nombre d’essais

## ✅ Exécution attendue

```yaml
Devine le nombre entre 1 et 100 :
> 50
C'est plus !
> 75
C'est moins !
> 63
Bravo ! Tu as trouvé en 3 essais.
```

## 🧠 Bonus

- Ajouter un système de score (nb d’essais) pour s'améliorer à chaque partie
- Proposer de rejouer une nouvelle partie automatiquement
- Ajouter un chronomètre (utiliser `System.currentTimeMillis()`)

## 🧩 Besoin d’un coup de pouce ?

😵‍💫 Bloqué ? Pas grave, on est là pour apprendre !