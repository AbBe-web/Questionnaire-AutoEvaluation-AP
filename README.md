README.md
```

---

# PAP-Plateforme

Outil de pré-consultation Activité Physique (patient)

---

## Description

PAP-Plateforme est un outil mono-fichier HTML destiné aux patients, permettant :

* L’évaluation du niveau d’activité physique (GPAQ – OMS / Marshall)
* Le calcul des MET-min/semaine
* La détermination du stade motivationnel
* L’auto-évaluation de l’importance et de la confiance (EVA 0–10)

Le résultat est destiné à être apporté en consultation médicale.
Aucune donnée n’est stockée.

---

## Architecture du projet

Le projet repose sur trois niveaux distincts :

### 1. Logique clinique (gelée)

Les éléments suivants sont strictement verrouillés :

* Questionnaires (GPAQ, Marshall)
* Calculs et seuils
* Logique motivationnelle
* Ordre des étapes
* Structure des résultats

Voir :
**PROTOCOLE_STABILITE_CLINIQUE_PAP.md**

---

### 2. Stabilité technique (anti-régression)

Toute correction ou modification technique suit un protocole DSR (Debug Sans Régression) visant à :

* Corriger sans perte fonctionnelle
* Éviter toute régression visible ou invisible
* Maintenir l’intégrité des parcours validés

Voir :
**PROTOCOLE_DSR_PAP.md**

---

### 3. Évolutions

Les évolutions majeures sont possibles uniquement après demande explicite et validation formelle.

---

## Caractéristiques techniques

* Application mono-fichier HTML
* Aucune base de données
* Aucun stockage persistant
* Exécution locale navigateur

---

## Gouvernance

Si ce n’est pas explicitement demandé, ce n’est pas modifié.

---
