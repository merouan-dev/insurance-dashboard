# 🎯 Tableau de Bord d'Assurance | Insurance Dashboard

[![GitHub Pages](https://img.shields.io/badge/demo-live-success?style=for-the-badge)](https://merouan-dev.github.io/insurance-dashboard/)
[![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)](LICENSE)

> Application web interactive pour la gestion et la visualisation des contrats d'assurance automobile au Maroc.

![Dashboard Preview](https://img.shields.io/badge/Status-Production-brightgreen?style=flat-square)

---

## 📋 Table des Matières

- [À Propos](#-à-propos)
- [Fonctionnalités](#-fonctionnalités)
- [Technologies](#-technologies-utilisées)
- [Installation](#-installation)
- [Utilisation](#-utilisation)
- [Structure du Projet](#-structure-du-projet)
- [Démo en Ligne](#-démo-en-ligne)
- [Auteur](#-auteur)
- [Licence](#-licence)

---

## 🎨 À Propos

Ce projet a été développé dans le cadre du parcours **Développement Digital - Web FullStack**. Il s'agit d'une application web moderne permettant de :

- 📊 Visualiser les statistiques des contrats d'assurance
- 🔍 Filtrer les données par ville, type d'assurance et type de véhicule
- 📥 Importer des fichiers Excel (XLSX) automatiquement ou manuellement
- 💾 Stocker les données localement dans le navigateur (IndexedDB)
- 📱 Interface responsive compatible mobile, tablette et desktop

---

## ✨ Fonctionnalités

### 🏠 Page d'Accueil
- Navigation intuitive vers l'application
- Téléchargement des fichiers Excel et PowerPoint
- Design moderne avec effets de hover
- Lien direct vers le repository GitHub

### 📊 Tableau de Bord Interactif
- **Indicateurs Clés (KPI)** :
  - Total des primes d'assurance
  - Nombre total de contrats
  - Ville la plus active
  - Nombre de clients VIP

- **Filtres Dynamiques** :
  - Filtrage par ville
  - Filtrage par type d'assurance (Tiers, Tiers+, Tous Risques)
  - Filtrage par type de véhicule (Voiture, Moto, Camion)

- **Visualisations** :
  - Graphiques de répartition des véhicules
  - Tableau détaillé avec toutes les informations clients
  - Mise à jour en temps réel lors du filtrage

### 💾 Gestion des Données
- **Chargement Automatique** : Charge le fichier par défaut depuis le serveur
- **Import Manuel** : Glisser-déposer ou sélection de fichier Excel
- **Persistance** : Sauvegarde automatique dans IndexedDB
- **Validation** : Vérification de l'intégrité des données importées

---

## 🛠️ Technologies Utilisées

### Frontend
- **HTML5** - Structure sémantique
- **CSS3** - Styles modernes avec animations
- **JavaScript (ES6+)** - Logique applicative
- **Bootstrap 5** - Framework CSS responsive

### Bibliothèques
- **jQuery** - Manipulation DOM simplifiée
- **SheetJS (xlsx.js)** - Lecture de fichiers Excel
- **Font Awesome** - Icônes vectorielles

### Stockage
- **IndexedDB** - Base de données locale du navigateur

### Hébergement
- **GitHub Pages** - Déploiement et hébergement gratuit

---

## 📥 Installation

### Prérequis
- Navigateur web moderne (Chrome, Firefox, Edge, Safari)
- Serveur local (optionnel pour le mode automatique)

### Étapes

1. **Cloner le repository**
```bash
git clone https://github.com/merouan-dev/insurance-dashboard.git
cd insurance-dashboard
```

2. **Option A : Ouvrir directement**
```bash
# Ouvrir index.html dans votre navigateur
# Note : Le chargement automatique ne fonctionnera pas en mode file://
```

3. **Option B : Utiliser un serveur local (recommandé)**
```bash
# Avec Python 3
python -m http.server 8000

# Avec Node.js (http-server)
npx http-server

# Avec VS Code
# Installer l'extension "Live Server" et cliquer sur "Go Live"
```

4. **Accéder à l'application**
```
http://localhost:8000
```

---

## 🚀 Utilisation

### 1. Accéder à l'Application
- Ouvrez `index.html` dans votre navigateur
- Cliquez sur **"Application Web"**

### 2. Charger les Données

#### Option A : Chargement Automatique
- Cliquez sur **"Chargement Automatique"**
- Le fichier `efm-merouan.xlsx` sera chargé automatiquement
- ⚠️ Nécessite un serveur local (http://)

#### Option B : Import Manuel
- Cliquez sur **"Import Manuel"**
- Glissez-déposez votre fichier Excel ou cliquez pour le sélectionner
- Le fichier doit contenir les colonnes requises (voir structure ci-dessous)

### 3. Explorer les Données
- Consultez les indicateurs clés en haut de page
- Utilisez les filtres pour affiner votre recherche
- Parcourez le tableau détaillé des contrats

---

## 📁 Structure du Projet

```
insurance-dashboard/
│
├── index.html                      # Page d'accueil
├── insurance_dashboard.html        # Application principale
├── efm-merouan.xlsx               # Fichier de données Excel
├── efm-merouan.pptx               # Présentation du projet
└── README.md                       # Documentation
```

### Structure des Données Excel

Le fichier Excel doit contenir les colonnes suivantes :

| Colonne | Description | Type |
|---------|-------------|------|
| `ID_Client` | Identifiant unique du client | Texte |
| `Nom` | Nom de famille | Texte |
| `Prenom` ou `Prénom` | Prénom | Texte |
| `CIN` | Numéro de carte d'identité | Texte |
| `Ville` | Ville du client | Texte |
| `Type_Vehicule` | Type de véhicule (Voiture, Moto, Camion) | Texte |
| `Marque` | Marque du véhicule | Texte |
| `Valeur_Vehicule` | Valeur du véhicule en MAD | Nombre |
| `Type_Assurance` | Type d'assurance (Tiers, Tiers+, Tous Risques) | Texte |
| `Prime_Base` | Prime de base | Nombre |
| `Taux_Risque` | Taux de risque (%) | Nombre |
| `Montant_Risque` | Montant du risque | Nombre |
| `Prime_Totale` | Prime totale | Nombre |
| `Statut_Client` | Statut (Standard, Premium, VIP) | Texte |
| `Date_Souscription` | Date de souscription | Date |
| `Duree_Contrat` | Durée du contrat (mois) | Nombre |

---

## 🌐 Démo en Ligne

🔗 **[Voir la démo live](https://merouan-dev.github.io/insurance-dashboard/)**

---

## 🎓 Contexte Académique

**Formation** : Développement Digital - Web FullStack  
**Formateur** : Said GAHI  
**Année** : 2025

---

## 👨‍💻 Auteur

**Merouan Errachidi**

- GitHub: [@merouan-dev](https://github.com/merouan-dev)
- Portfolio: [merouan-dev.github.io](https://merouan-dev.github.io)

---

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

## 🙏 Remerciements

- **Said GAHI** - Formateur et encadrant du projet
- **Bootstrap Team** - Pour le framework CSS
- **SheetJS** - Pour la bibliothèque de traitement Excel
- **Font Awesome** - Pour les icônes

---

## 📞 Support

Pour toute question ou suggestion :
- Ouvrir une [issue](https://github.com/merouan-dev/insurance-dashboard/issues)
- Contacter via GitHub

---

<div align="center">

**⭐ Si ce projet vous a été utile, n'hésitez pas à lui donner une étoile !**

Made with ❤️ by Merouan Errachidi

</div>
