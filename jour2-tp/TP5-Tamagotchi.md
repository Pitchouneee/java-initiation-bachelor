# TP5 – 🐣 Tamagotchi CLI

**Objectifs :** Approfondir la POO avec un objet à état évolutif

## 🎓 Cours lié : État interne d’un objet et encapsulation

Ce TP te plonge dans la **programmation orientée objet vivante** : tu vas modéliser une petite créature virtuelle avec des **états internes dynamiques** qui évoluent selon les actions de l’utilisateur.

C’est l’occasion parfaite pour pratiquer :
- La **modélisation d’un objet vivant**
- La gestion de son **état interne**
- L’**encapsulation** (principe clé de la POO)
- L’interaction via un **menu console**

### 🧬 L’état d’un objet

Un objet possède des **attributs** qui représentent son état actuel.

Exemple avec un Tamagotchi :

```java
public class Tamagotchi {
    private int faim;
    private int energie;
    private int bonheur;
}
```

### 🧪 Le constructeur : initialiser ton objet

Tu peux créer un `constructeur` pour initialiser les états :

```java
public Tamagotchi() {
    this.faim = 50;
    this.energie = 50;
    this.bonheur = 50;
}
```

> 🎯 À la création, tous les Tamagotchis commencent à mi-énergie / mi-faim / mi-joie.

### ⚙️ Encapsulation : protéger les données

Les attributs sont souvent déclarés en `private` pour *protéger* l’état de l’objet. On les modifie via des méthodes publiques :

```java
public void manger() {
    faim -= 10;
    energie += 5;
}
```

Et pour afficher :

```java
public void afficherStatut() {
    System.out.println("Faim : " + faim);
    System.out.println("Énergie : " + energie);
    System.out.println("Bonheur : " + bonheur);
}
```

> [!NOTE]
> 🔐 L’encapsulation évite les modifications directes incontrôlées, et te permet de garder un **contrôle métier** (ex. : pas de faim négative).

### 🔁 Menu console et boucle de jeu

Tu peux proposer un menu d’actions en boucle, comme dans un vrai jeu CLI :

```yaml
1 – Manger  
2 – Dormir  
3 – Jouer  
4 – Quitter
```

Et utiliser une boucle `while` ou `do-while` pour répéter tant que l’utilisateur ne quitte pas.

## 🎯 Objectifs du TP

Approfondir la programmation orientée objet (POO) en créant un objet à **état évolutif**.

Fonctionnalités attendues :
- Créer une classe `Tamagotchi` avec les attributs : `faim`, `énergie`, `bonheur`
- Implémenter les méthodes : `manger()`, `dormir()`, `jouer()` qui modifient l’état
- Afficher le statut après chaque action
- Proposer un menu en boucle jusqu’à ce que le joueur quitte

## ✅ Exécution attendue

```yaml
Que veut faire ton Tamagotchi ?
1 - Manger
2 - Dormir
3 - Jouer
4 - Quitter
> 1
[Le Tamagotchi mange 🍎]

Statut :
Faim : 40
Énergie : 55
Bonheur : 50
```

## 🧠 Bonus

- Ajouter une animation ASCII ou un petit visuel d’humeur
- Introduire une durée de vie limitée ou un "game over"
- Sauvegarder la progression dans un fichier

## 🧩 Besoin d’un coup de pouce ?

🧃 Ton Tamagotchi est perdu ? Ton intervenant est là pour le nourrir !

📘 **Pour aller plus loin :**

- 📦 [TP7 – Structurer son projet Java](../bonus/TP7-Packages-et-organisation.md) : transforme ton jeu Tamagotchi en vrai projet Java modulaire