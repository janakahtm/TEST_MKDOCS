# Création basique d'une liste

```python title="Liste en python"
def creer_et_afficher_liste():
"""Crée et affiche une liste d'étudiants"""
etudiants = ["Alice", "Bob", "Charlie", "Diana"]

    print("📋 Liste des étudiants:")
    print("-" * 20)

    for etudiant in etudiants:
        print(f"• {etudiant}")

    return etudiants
```

### Exécution

```
ma_liste_etudiants = creer_et_afficher_liste()

print(f"\nNombre d'étudiants: {len(ma_liste_etudiants)}")
```

```python title="Python"
print("Hello World!")
```

```javascript title="JavaScript"
console.log("Hello World!");
```

```java title="Java"
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

```
sudo apt update
sudo apt install vi
```

```python
def greet(name):
    print(f"Hello, {name}")
```

```java
class Hello {
  public static void main(String[] args) {
    System.out.println("Hi");
  }
}
```

```bash
# Met à jour l’index des paquets (commentaire -> couleur)
sudo apt update

# Installe vim (option -y -> couleur ; chaîne -> couleur)
sudo apt install -y vim
echo "OK" | tee ~/install.log

# Variables et substitution -> couleurs
PKG="vim"; sudo apt install "$PKG"
```
