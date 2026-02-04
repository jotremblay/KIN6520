# KIN6520 – Laboratoire I : Analyse d'un test VO₂max

Bienvenue dans le dépôt du Laboratoire I. Vous y trouverez tout le matériel nécessaire pour compléter votre rapport.

---

## 1. Télécharger les fichiers

### Option recommandée : Télécharger le ZIP

1. Cliquez sur le bouton vert **Code** (en haut à droite de cette page)
2. Sélectionnez **Download ZIP**
3. Décompressez le fichier ZIP sur votre ordinateur
4. Ouvrez le dossier `KIN6520-main` dans Positron (ou RStudio)

### Option alternative : Cloner avec Git

Si vous êtes à l'aise avec Git :

```bash
git clone https://github.com/VOTRE-URL/KIN6520.git
```

---

## 2. Trouver votre fichier de données

Chaque étudiant analyse un fichier différent. Trouvez votre matricule ci-dessous :

| Matricule | Fichier |
|-----------|---------|
| 20191697 | `P01` |
| 20207125 | `P02` |
| 20209486 | `P03` |
| 20231812 | `P04` |
| 20236944 | `P05` |
| 20238321 | `P06` |
| 20242392 | `P07` |
| 20245501 | `P08` |
| 20271197 | `P09` |
| 20325870 | `P10` |
| 20327827 | `P11` |
| 20337811 | `P12` |
| 20338693 | `P13` |
| 20355889 | `P14` |
| 20359534 | `P15` |

Les fichiers se trouvent dans le dossier :

```
data/student_files/
```

---

## 3. Compléter votre rapport

### Étape 1 : Ouvrir le gabarit

Ouvrez le fichier `rapport.qmd` dans Positron.

### Étape 2 : Indiquer votre fichier de données

Au tout début du document, vous verrez cette section :

```r
# ============================================================================
# VOTRE FICHIER DE DONNÉES
# ============================================================================
# Consultez le README pour trouver votre fichier selon votre matricule.
# Modifiez la ligne ci-dessous avec votre numéro de fichier (P01 à P15) :

mon_fichier <- "P01"
```

**Remplacez `"P01"` par votre fichier assigné** (ex: `"P07"`, `"P12"`, etc.)

### Étape 3 : Générer le rapport

Cliquez sur **Render** pour exécuter le code et générer votre rapport HTML.

---

## 4. Structure du dépôt

```
KIN6520/
├── README.md              ← Vous êtes ici
├── rapport.qmd            ← Gabarit de votre rapport (à compléter)
├── en_classe.qmd          ← Document utilisé pendant la séance en classe
├── data.xlsx              ← Fichier exemple pour en_classe.qmd
│
└── data/
    └── student_files/     ← VOS FICHIERS DE DONNÉES
        ├── P01.xlsx
        ├── P02.xlsx
        ├── ...
        └── P15.xlsx
```

---

## 5. Contenu des fichiers de données

Chaque fichier Excel (P01.xlsx, P02.xlsx, etc.) contient 3 feuilles :

| Feuille | Description |
|---------|-------------|
| `Data` | Données respiration par respiration : VO₂, VCO₂, FC, VE, RER, vitesse, etc. |
| `Participant` | Informations anonymisées : ID, sexe, âge, taille, poids |
| `Results` | Résumé des résultats du logiciel COSMED |

---

## 6. Packages R requis

Si vous n'avez pas encore ces packages, installez-les :

```r
install.packages(c("tidyverse", "readxl", "zoo"))
```

---

## Questions?

Posez vos questions sur le **forum StudiUM** du cours. Cela permet à tout le monde de bénéficier des réponses.
