# 🎯 Tableau de Bord d'Assurance

> Application web interactive pour la gestion et la visualisation des contrats d'assurance automobile au Maroc.

[![Live Demo](https://img.shields.io/badge/demo-live-success?style=for-the-badge)](https://merouan-dev.github.io/insurance-dashboard/)

---

## 🚀 Démo en Ligne

**[👉 Accéder à l'application](https://merouan-dev.github.io/insurance-dashboard/)**

---

## ✨ Fonctionnalités

- 📊 **Dashboard interactif** avec indicateurs clés (KPI)
- 🔍 **Filtres dynamiques** par ville, type d'assurance et véhicule
- 📥 **Import Excel** automatique ou manuel (XLSX)
- 💾 **Stockage local** avec IndexedDB
- � **Design responsive** (mobile, tablette, desktop)
- 🎨 **Interface moderne** avec animations

---

## 🛠️ Technologies

- **HTML5** / **CSS3** / **JavaScript (ES6+)**
- **Bootstrap 5** - Framework CSS
- **jQuery** - Manipulation DOM
- **SheetJS** - Lecture de fichiers Excel
- **IndexedDB** - Base de données locale
- **Font Awesome** - Icônes

---

## 📥 Installation

```bash
# Cloner le repository
git clone https://github.com/merouan-dev/insurance-dashboard.git
cd insurance-dashboard

# Ouvrir avec un serveur local (recommandé)
python -m http.server 8000
# ou
npx http-server

# Accéder à http://localhost:8000
```

---

## � Structure des Données Excel

Le fichier Excel doit contenir ces colonnes :

- `ID_Client`, `Nom`, `Prenom`, `CIN`, `Ville`
- `Type_Vehicule`, `Marque`, `Valeur_Vehicule`
- `Type_Assurance`, `Prime_Base`, `Prime_Totale`
- `Statut_Client`, `Date_Souscription`, `Duree_Contrat`

---

## 👨‍💻 Auteur

**Merouan Errachidi**  
GitHub: [@merouan-dev](https://github.com/merouan-dev)

**Formateur : Said GAHI**

---

## 📄 Licence

MIT License - Projet académique 2025

---

<div align="center">

**⭐ N'hésitez pas à donner une étoile si ce projet vous plaît !**

Made with ❤️ by Merouan Errachidi

</div>
