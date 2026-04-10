<p align="center">
  <h1>🍔 BK AutoSurvey</h1>
  <p><b>Automatisation intelligente des enquêtes Burger King (Qualtrics)</b></p>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-success?style=for-the-badge">
  <img src="https://img.shields.io/badge/javascript-vanilla-yellow?style=for-the-badge">
  <img src="https://img.shields.io/badge/license-personal--use-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/made%20with-%E2%9D%A4-red?style=for-the-badge">
</p>

---

## 📖 Présentation

**BK AutoSurvey** automatise entièrement le remplissage des enquêtes clients Burger King basées sur Qualtrics.

- Plus besoin de répondre manuellement  
- Le script s’occupe de tout  
- Récupération automatique du code de réduction final  

---

## 🤖 Fonctionnalités

- Génération instantanée de script (bookmarklet / console)  
- Remplissage automatique complet du questionnaire  
- Détection des pages et transitions  
- Panneau de suivi en temps réel (logs + progression)  
- Extraction automatique du code de validation  
- Facilement adaptable si le formulaire évolue  

---

## 🖼️ Aperçu

<p align="center">
  <img width="800" src="https://github.com/user-attachments/assets/e79ebf0a-a0d8-4af4-9230-201251c2db05" />
  <img width="800" src="https://github.com/user-attachments/assets/3b16f07d-86c5-4f67-bcd2-0c730c7078f0" />
  <img width="600" src="https://github.com/user-attachments/assets/f00820f3-5dec-4a86-b0cb-82ea397e121e" />
  <img width="300" src="https://github.com/user-attachments/assets/8eb7b5db-d953-465e-8ddf-606f1ece63a1" />
</p>

---

## 🛠️ Utilisation

### 1️ - Génération

Renseignez :

- numéro du restaurant  
- date / heure  
- commentaire  

Puis cliquez sur **"Générer"**

---

### 2️ - Accès au formulaire Qualtrics ⚠️

Le lien réel du questionnaire est caché derrière :  
    https://www.bkvousecoute.fr/

---

### 🔍 Récupérer le lien Qualtrics

1. Ouvrir le site  
2. Appuyer sur `F12`  
3. Aller dans l’onglet **Network**  
4. Recharger la page (`F5`)  
5. Filtrer :
    qualtrics
    ou
    jfe/form
6. Copier une URL du type :
    https://xxxxx.qualtrics.com/jfe/form/SV_XXXXXXXX
7. Ouvrir dans un nouvel onglet  

---

### 3️ - Exécution

#### Méthode A — Bookmarklet

- Glisser le bouton dans les favoris  
- Cliquer dessus depuis la page Qualtrics  

#### Méthode B — Console

- `F12` → Console  
- Coller le script → Entrée  

---

### 4️ - Résultat

Le script va :

- Naviguer automatiquement  
- Répondre à toutes les questions  
- Simuler une saisie réaliste  
- Afficher le code promo final  

---

## ⚙️ Configuration avancée

### Lien Qualtrics par défaut

const QURL = "https://rbixm.qualtrics.com/jfe/form/SV_9MHgHFvPm0OEHr0?CountryCode=FRA&Q_Language=FR&PT=1";

Modifier le lien si nécessaire

Fonctionnement interne :
- Injection JavaScript dans la page Qualtrics
- Analyse dynamique du DOM
- Sélection automatique des réponses
- Gestion des transitions multi-pages
- Hook sur les événements Qualtrics
- Extraction du code final

Temps d’exécution

~15 à 30 secondes

---

## Disclaimer :
- Projet non officiel Burger King
- Usage éducatif uniquement

Peut cesser de fonctionner si :
- modification du formulaire
- changement des IDs Qualtrics
- protection anti-bot renforcée

---
