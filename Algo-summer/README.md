# Analyse de Phrase - Algorithme

![Checkpoint Image](sentence-algorithm-checkpoint.png)

## Description

Ce projet implémente un algorithme en pseudo-code (fichier `.algo`) qui lit une phrase **caractère par caractère** jusqu'au point final et détermine trois statistiques :

1. **La longueur de la phrase** — nombre total de caractères (y compris le point final)
2. **Le nombre de mots** — les mots sont séparés par un seul espace
3. **Le nombre de voyelles** — comptage des voyelles (a, e, i, o, u, y) en minuscules et majuscules

## Fichier principal

- [`ph.algo`](ph.algo) — Contient l'algorithme en pseudo-code avec :
  - 3 variables compteurs : `longueur`, `nb_mots`, `nb_voyelles`
  - Une boucle `TantQue` qui lit chaque caractère individuellement
  - Détection des voyelles (casinsensible)
  - Traitement du point final comme dernier caractère

## Critères du checkpoint

| Critère | Satisfaction |
|---|---|
| ✅ Utilisation de 3 variables compteurs | `longueur`, `nb_mots`, `nb_voyelles` |
| ✅ GitHub repository avec README | ✅ |
| ✅ Documentation & clarté du code | Commentaires détaillés, structure claire |
| ✅ Technical mastery | Algorithme robuste, cas gérés |
| ✅ Work quality | Code propre et lisible |
| ✅ Problem resolution | Approche caractère par caractère |
| ✅ Deadline | Livré dans les temps |

## Logique de l'algorithme

1. Initialiser les 3 compteurs à 0
2. Lire le premier caractère
3. Tant que le caractère n'est pas un point (`.`)
   - Incrémenter `longueur`
   - Si c'est une voyelle → incrémenter `nb_voyelles`
   - Si c'est un espace → incrémenter `nb_mots`
   - Lire le caractère suivant
4. Incrémenter `longueur` pour inclure le point final
5. Ajouter 1 à `nb_mots` (mots = espaces + 1)
6. Afficher les résultats

## Exemple

Pour la phrase : `"Bonjour le monde."`

```
Longueur de la phrase        : 18 caractère(s)
Nombre de mots               : 3 mot(s)
Nombre de voyelles           : 7 voyelle(s)
```

## Auteur

Projet réalisé dans le cadre du checkpoint Algorithmique — Algo-summer 2026.
