# Oracle Géomantique (Algorithme de Divination)

Bienvenue dans le dépôt du projet **Oracle Géomantique**, un programme informatique conçu pour simuler, générer et interpréter les figures de la géomancie traditionnelle.

## 🔮 Qu'est-ce que la Géomancie ?
La géomancie (du grec *ge*, la terre, et *manteia*, la divination) est un art divinatoire traditionnel qui consiste à interpréter des marques tracées sur le sol ou, dans notre cas, générées aléatoirement par un algorithme. Le système repose traditionnellement sur 16 figures géomantiques composées de combinaisons de 1 à 2 points (lignes simples ou doubles), réparties sur 4 hauteurs. 

Cet algorithme automatise la création des figures mères, des nièces, des compagnes, du juge et des témoins pour aboutir à une interprétation structurée.

---

## 🚀 Fonctionnalités principales
- **Génération aléatoire authentique :** Simulation de tirages de points (par jet de dés, saisie utilisateur ou générateur pseudo-aléatoire).
- **Calcul des figures dérivées :** 
  - Les 4 figures mères
  - Les 4 nièces et les 4 compagnes
  - Les témoins (gauche et droit) et le Juge
  - Le futur / La sentence (Seconde Juge / Bouche de la fosse, selon les variantes)
- **Moteur d'interprétation :** Association des figures à des significations traditionnelles.
- **Interface CLI / API :** Utilisation en ligne de commande ou intégration modulaire.

---

## 🛠️ Installation et Prérequis

Assurez-vous d'avoir l'environnement nécessaire installé sur votre machine (par exemple, Python 3.x ou Node.js selon votre stack).

```bash
# Cloner le dépôt
git clone https://github.com/votre-nom-utilisateur/nom-du-projet.git

# Accéder au dossier du projet
cd nom-du-projet

# Installer les dépendances (exemple pour Python)
pip install -r requirements.txt
```

---

## 💻 Utilisation

Exécutez le script principal pour lancer une consultation divinatoire :

```bash
python main.py
```

Exemple de sortie dans le terminal :
```text
=== TIRAGE GÉOMANTIQUE ===
Mères : [Puer] [Albus] [Amissio] [Fortuna Major]
...
Le Juge : [Acquisitio]
Interprétation : Succès financier et gains matériels en perspective.
```

---

## 📂 Structure du Projet

```text
├── src/
│   ├── figures.py      # Définition des 16 figures géomantiques et de leurs propriétés
│   ├── generator.py    # Logique de tirage et de calcul des matrices (mères, nièces, etc.)
│   └── interpreter.py  # Dictionnaire des sens et génération du rapport
├── tests/              # Tests unitaires pour valider les calculs mathématiques des figures
├── main.py             # Point d'entrée de l'application
├── requirements.txt    # Dépendances du projet
└── README.md           # Documentation
```

---

## 🤝 Contribuer
Les contributions sont les bienvenues ! Que ce soit pour améliorer l'exactitude historique et ésotérique des algorithmes, optimiser le code ou enrichir le dictionnaire d'interprétation :
1. Forkez le projet
2. Créez votre branche (`git checkout -b feature/AmeliorationInterpretation`)
3. Committez vos changements (`git commit -m 'Ajout d'une nouvelle règle de calcul'`)
4. Poussez vers la branche (`git push origin feature/AmeliorationInterpretation`)
5. Ouvrez une Pull Request

---

## 📄 Licence
Distribué sous la licence MIT. Voir `LICENSE` pour plus d'informations.