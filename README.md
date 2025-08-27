# Gestion des Polynômes Réels avec Listes Doublement Chaînées 📊

Un programme C++ implémentant une structure de données de liste doublement chaînée pour la représentation et la manipulation de polynômes réels.

## 👥 Auteurs

- **TRAORE Souleymane**
- **RACHIDI OUSSAMA**
- **Date :** 18 avril 2023
- **Version :** 1.0

## 📋 Description du Projet

Ce projet est un devoir libre qui démontre l'implémentation d'une liste doublement chaînée en C++ et son application pratique pour la gestion de polynômes réels. Le programme permet de créer, manipuler et effectuer diverses opérations sur les polynômes.

## 🎯 Objectifs Pédagogiques

- Maîtriser les structures de données dynamiques (listes doublement chaînées)
- Comprendre la gestion de la mémoire en C++
- Appliquer les concepts théoriques à un cas pratique (polynômes)
- Développer des algorithmes de manipulation de données structurées

## 🏗️ Structure du Programme

### Partie 1 : Gestion des Listes Doublement Chaînées

**Structures de données :**
```cpp
typedef struct {
    double coefficient;
    int exposant;
} Monome;

typedef struct cellule {
    TypeListe donnee;
    struct cellule * suivant;
    struct cellule * precedent;
} Cellule;

typedef struct {
    Cellule * debut;
    Cellule * fin;
} Liste;
```

**Opérations de base :**
- Initialisation de liste vide
- Ajout en début et fin de liste
- Suppression en début et fin de liste

### Partie 2 : Application aux Polynômes Réels

**Fonctionnalités implémentées :**
- Création et initialisation de polynômes
- Saisie interactive de polynômes
- Affichage formaté des polynômes
- Calcul du degré d'un polynôme
- Ajout et suppression de monômes

## ✨ Opérations Mathématiques Disponibles

### Opérations Arithmétiques
- **Addition** de deux polynômes
- **Soustraction** de deux polynômes
- **Multiplication** de deux polynômes
- **Opposé** d'un polynôme

### Opérations d'Évaluation
- **Évaluation classique** : calcul de P(x) pour une valeur donnée
- **Évaluation par méthode de Horner** : méthode optimisée

### Opérations Avancées
- **Division euclidienne** de polynômes
- **Gestion des monômes** (ajout/suppression avec fusion automatique)

## 🚀 Compilation et Exécution

### Prérequis
- Compilateur C++ (g++, clang++, ou équivalent)
- Support C++11 ou supérieur

### Compilation
```bash
g++ -o polynomes devoir_libre_polynomes.cpp -lm
```

### Exécution
```bash
./polynomes
```

## 📖 Guide d'Utilisation

Le programme propose un menu interactif avec les options suivantes :

1. **Création d'un polynôme** : Saisie des coefficients et exposants
2. **Ajout de monômes** : Insertion de nouveaux termes
3. **Suppression de monômes** : Retrait de termes par exposant
4. **Opérations arithmétiques** : Addition, soustraction, multiplication
5. **Évaluation** : Calcul de la valeur du polynôme en un point
6. **Calcul de l'opposé** : Inversion des signes

### Exemple d'utilisation
```
Donner le couple coefficients et exposants (0 ou exposant négatif pour arrêter) : 
3 2    // 3x²
-2 1   // -2x
5 0    // +5
0 -1   // Arrêt de la saisie

Résultat : 3x² - 2x + 5
```

## 🛠️ Fonctionnalités Techniques

### Gestion Mémoire
- Allocation dynamique avec `new` et `delete`
- Libération automatique de la mémoire
- Gestion des pointeurs NULL

### Algorithmes Optimisés
- **Insertion ordonnée** : les monômes sont automatiquement triés par exposant décroissant
- **Fusion de monômes** : les termes de même exposant sont automatiquement combinés
- **Méthode de Horner** : évaluation efficace des polynômes

### Robustesse
- Gestion des cas particuliers (listes vides, polynômes nuls)
- Vérification des pointeurs avant utilisation
- Nettoyage automatique de la mémoire

## 🔧 Améliorations Possibles

- Ajout d'une interface graphique
- Implémentation de la dérivation et intégration
- Support des polynômes à coefficients complexes
- Optimisation des performances pour les gros polynômes
- Ajout de tests unitaires automatisés

## 📚 Concepts Mathématiques Utilisés

- **Polynômes réels** : représentation et propriétés
- **Opérations algébriques** : addition, multiplication, division
- **Évaluation de Horner** : méthode d'évaluation optimisée
- **Division euclidienne** : algorithme de division de polynômes

## 🐛 Limitations Connues

- La fonction de division euclidienne nécessite des améliorations
- Gestion limitée des erreurs de saisie utilisateur
- Affichage qui pourrait être amélioré pour les coefficients négatifs

## 📄 Structure des Fichiers

```
projet/
├── devoir_libre_polynomes.cpp    # Code source principal
├── README.md                     # Cette documentation
└── exemples/                     # (optionnel) Exemples d'exécution
```

## 🎓 Contexte Académique

Ce projet s'inscrit dans le cadre de l'apprentissage des structures de données et de leur application pratique. Il illustre :

- L'implémentation de structures de données complexes
- La résolution de problèmes mathématiques par programmation
- Les bonnes pratiques de développement en C++
- La gestion de la mémoire dynamique

## 📞 Contact

Pour toute question concernant ce projet :
- **TRAORE Souleymane**
- **RACHIDI OUSSAMA**

---
*Projet réalisé dans le cadre d'un devoir libre - 2023*
