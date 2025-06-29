# TP3 – ⏰ Horloge numérique

**Objectifs :** Travailler les boucles, les délais et l’affichage dynamique en console

## 🎓 Cours lié : Boucles infinies, temps système et pause d’exécution

Dans ce TP, tu vas apprendre à :
- Faire tourner un programme **en continu**
- **Afficher l’heure actuelle** en direct
- Ajouter une **pause régulière** pour simuler le temps réel

L’occasion parfaite de combiner boucles, gestion du temps et affichage dynamique ⏳

📚 Pour aller plus loin :

- [Documentation `LocalTime`](https://docs.oracle.com/en/java/javase/21/docs/api/java.base/java/time/LocalTime.html)
- [`Thread.sleep()` – Oracle JavaDoc](https://docs.oracle.com/en/java/javase/21/docs/api/java.base/java/lang/Thread.html#sleep(long))

### 🔁 Boucles infinies

En Java, une boucle while(true) permet de répéter une action sans fin, tant qu’une condition est vraie.

```java
while (true) {
    System.out.println("Je tourne à l'infini !");
}
```

> [!WARNING]  
> Attention : une boucle infinie doit être **maîtrisée**, sinon elle peut bloquer votre programme.

### ⏰ Obtenir l’heure système

Java fournit la classe `LocalTime` pour connaître l’heure actuelle :

```java
import java.time.LocalTime;

LocalTime maintenant = LocalTime.now();
System.out.println(maintenant); // Affiche : 14:53:07.123456
```

### 🧽 Formatage de l’heure

On peut formater proprement l’heure avec `DateTimeFormatter` :

```java
import java.time.format.DateTimeFormatter;

DateTimeFormatter format = DateTimeFormatter.ofPattern("HH:mm:ss");
System.out.println(maintenant.format(format)); // Exemple : 14:53:07
```

### 😴 Faire une pause dans l’exécution

Pour créer une attente entre chaque affichage, on utilise :

```java
Thread.sleep(1000); // Pause de 1000 ms = 1 seconde
```

> [!NOTE]  
> Cette méthode peut lancer une exception (`InterruptedException`), donc il faut l’entourer d’un bloc `try/catch`.

## 🎯 Objectifs du TP

Tu vas créer une horloge numérique qui :

- Affiche l’heure actuelle au format `HH:mm:ss` dans la console
- Met à jour toutes les secondes
- Fonctionne en temps réel (boucle infinie avec pause)

## ✅ Exécution attendue

```yaml
Il est actuellement 09:42:27
```

## 🧠 Bonus

- Ajouter la date (avec `LocalDate`)

## 🧩 Besoin d’un coup de pouce ?

🤯 Le bug fait partie du jeu — demande un coup de main