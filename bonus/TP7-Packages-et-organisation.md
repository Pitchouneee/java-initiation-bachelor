# TP7 – 📦 Structurer un projet Java

**Objectifs :** Organiser son code Java comme un vrai projet

## 🧱 Problème à résoudre

Ton fichier `Main.java` contient tout le code ? 😅 Il est temps de **séparer** les responsabilités !

## 📁 Objectif

Réorganiser un TP précédent (ex. TP4 ou TP5) en :

```bash
src/
 ┣ Main.java
 ┣ model/
 ┃ ┗ Livre.java
 ┗ service/
   ┗ Bibliotheque.java
```

## 🎯 Étapes proposées

1. Créer le dossier `src/`
2. Créer les sous-dossiers `model/` et `service/`
3. Placer chaque classe dans un fichier propre avec la bonne ligne `package`
4. Compiler avec :
```bash
javac -d bin src/**/*.java
```
5. Lancer le programme avec :
```bash
java -cp bin Main
```

## 🔧 Exemple de package dans Livre.java

```java
package model;

public class Livre {
    // ...
}
```

Et dans `Main.java` :

```java
import model.Livre;
import service.Bibliotheque;
```
