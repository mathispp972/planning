# 📝 CHANGELOG - Training Planner

## Version 1.0 (15 février 2026)

### 🎉 Première Version Stable

Cette version marque la première release stable du Training Planner, prête pour une utilisation quotidienne !

---

## ✨ Fonctionnalités Principales

### 📅 Gestion de Séances
- ✅ Calendrier interactif mensuel
- ✅ 4 types de séances : Running🏃‍➡️, Musculation💪, Hyrox🤖, Cardio❤️‍🔥
- ✅ Création, édition, suppression de séances
- ✅ Copie de séances existantes pour gagner du temps
- ✅ Cycles d'entraînement (Force, Hypertrophie, Endurance)
- ✅ Commentaires par séance

### 💪 Gestion d'Exercices

#### Musculation & Hyrox
- ✅ Base de données d'exercices personnalisable
- ✅ Suivi par série avec :
  - Nombre de répétitions
  - Charge (kg)
  - RPE (1-10)
  - Validation par série (✅/⏳)
- ✅ **Nombre de séries par défaut : 4**
- ✅ Calcul automatique du 1RM (formule Brzycki)
- ✅ Affichage du meilleur 1RM parmi toutes les séries
- ✅ Indicateur de progression (séries validées)

#### Cardio & Running
- ✅ Distance (m ou km)
- ✅ Temps (MM:SS ou HH:MM:SS)
- ✅ Calcul automatique de l'allure
- ✅ Nombre de tours (pour fractionné)

### 📊 Statistiques & Progression
- ✅ Vue mensuelle des séances
- ✅ Total par type d'activité
- ✅ Graphiques de progression 1RM
- ✅ Sélection multi-exercices
- ✅ Exercices groupés par muscle

### ☁️ Synchronisation Google Drive

#### Connexion
- ✅ Authentification OAuth 2.0 sécurisée
- ✅ Token sauvegardé localement

#### Contrôle Manuel (pas de sync auto)
- ✅ **Bouton "⬇️ Charger depuis Drive"** : Récupère les données de Drive
  - Affiche un résumé avant de charger
  - Demande confirmation
  - Nombre de séances comparé (local vs Drive)
  - Date de dernière modification
  
- ✅ **Bouton "⬆️ Sauvegarder sur Drive"** : Envoie les données vers Drive
  - Confirmation avant écrasement
  - Mise à jour du fichier existant
  - Création si premier usage

- ✅ **Bouton "🔌 Déconnecter"** : Déconnexion de Drive
  - Données locales conservées

#### Gestion Intelligente
- ✅ Détection et suppression automatique des fichiers dupliqués
- ✅ Un seul fichier `training_planner_data.json` sur Drive
- ✅ Pas de synchronisation automatique (contrôle total)

### 📊 Export de Données
- ✅ Export Excel (.xlsx) avec 5 feuilles :
  1. Vue d'ensemble des séances
  2. Détail de tous les exercices
  3. Détail série par série (avec RPE)
  4. Statistiques mensuelles
  5. Base d'exercices

### 🎨 Interface Utilisateur
- ✅ Design moderne et responsive
- ✅ Mode sombre
- ✅ Optimisé mobile (utilisation en salle)
- ✅ Navigation par onglets
- ✅ Badges colorés par type de séance
- ✅ Indicateurs visuels (1RM, progression, validation)

### 🔧 Organisation
- ✅ Séances de musculation :
  - Dos/Epaules/Biceps🦍
  - Pecs/Epaules/Triceps👕
  - Epaules/Abdos🍫
  - Haut du corps⬆️
  - Bas du corps⬇️
  - Full Body🏋️

- ✅ Groupes musculaires (ordre alphabétique) :
  - Abdos, Abducteurs, Adducteurs
  - Biceps, Dos, Épaules
  - Fessiers, Ischio-jambiers, Jambes
  - Mollets, Pecs, Quadriceps, Triceps

---

## 🔄 Workflow Recommandé

### Premier Démarrage
1. Ouvrir l'app (GitHub Pages)
2. Se connecter à Google Drive
3. Créer ses premières séances
4. Sauvegarder sur Drive (⬆️)

### Utilisation Quotidienne
1. Ouvrir l'app
2. Charger depuis Drive (⬇️) - pour avoir la dernière version
3. Ajouter/modifier des séances
4. Sauvegarder sur Drive (⬆️) - avant de fermer

### Multi-Appareils
- **PC** : Planification et création de programmes
- **Téléphone** : Utilisation en salle de sport
- Synchronisation manuelle via boutons Drive

---

## 🛠️ Technologies Utilisées

- **Frontend** : HTML5, CSS3, JavaScript (Vanilla)
- **Graphiques** : Chart.js
- **Export Excel** : SheetJS (xlsx)
- **Cloud** : Google Drive API v3
- **Auth** : Google OAuth 2.0
- **Hébergement** : GitHub Pages

---

## 📦 Fichiers de la V1

- `training_planner_V1.html` : Application complète (fichier unique)
- `CHANGELOG.md` : Ce fichier
- `GUIDE_GOOGLE_DRIVE.md` : Guide de configuration Google Drive
- `CONFIG_RAPIDE_GDRIVE.md` : Configuration rapide
- `GUIDE_EXPORT_EXCEL.md` : Documentation export Excel
- `IDEES_FONCTIONNALITES.md` : Roadmap futures fonctionnalités

---

## ⚙️ Configuration Requise

### Pour l'Utilisation
- Navigateur moderne (Chrome, Firefox, Safari, Edge)
- Connexion Internet (pour Google Drive)
- Compte Google (optionnel, pour la synchronisation)

### Pour l'Hébergement
- Repository GitHub (public ou privé)
- GitHub Pages activé OU Netlify/Vercel

### Pour Google Drive
- Projet Google Cloud Platform
- API Google Drive activée
- Client ID OAuth 2.0
- API Key

---

## 🚀 Déploiement

1. Upload `training_planner_V1.html` sur GitHub
2. Activer GitHub Pages
3. Configurer Google Cloud (CLIENT_ID + API_KEY)
4. Accéder via l'URL GitHub Pages

---

## 🐛 Bugs Connus & Limitations

### Limitations
- Synchronisation manuelle uniquement (pas de sync temps réel)
- Un seul utilisateur par instance
- Stockage local limité par le navigateur

### Aucun Bug Critique Connu
La V1 est stable et testée ! ✅

---

## 🔮 Roadmap V2

Voir `IDEES_FONCTIONNALITES.md` pour la liste complète.

### Top 5 Priorités
1. Templates de séances réutilisables
2. Suggestions automatiques de charges
3. Timer de repos intégré
4. Planification programmes 4-12 semaines
5. Dashboard statistiques avancé

---

## 📄 Licence

Projet personnel - Mathis

---

## 👤 Crédits

**Développeur** : Mathis  
**Assistant IA** : Claude (Anthropic)  
**Date** : 15 février 2026

---

## 🙏 Remerciements

- Chart.js pour les graphiques
- SheetJS pour l'export Excel
- Google pour l'API Drive
- GitHub pour l'hébergement

---

**🎉 Version 1.0 - Stable & Prête pour Production ! 🎉**
