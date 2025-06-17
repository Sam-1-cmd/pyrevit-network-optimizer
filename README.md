# pyrevit-network-optimizer

# 🛠️ Génération intelligente de conduits dans Revit avec PyRevit

🎓 Projet réalisé dans le cadre de ma formation à l’ESTP Paris, option Jumeaux Numériques et Intelligence Artificielle.

## 🎯 Objectif

Développer un outil PyRevit permettant de tracer automatiquement un conduit 3D entre deux éléments du modèle Revit (ex. bouche d’aération et gaine), tout en détectant les obstacles (murs, poutres, etc.) et en calculant un chemin de contournement optimisé.

## ⚙️ Fonctionnalités

✅ Sélection de deux éléments MEP dans Revit  
✅ Calcul de leurs centres via la Revit API  
✅ Détection des obstacles à l’aide de `ReferenceIntersector`  
✅ Génération de points intermédiaires intelligents pour éviter les collisions  
✅ Création de conduits 3D (DirectShape) avec matériau et rayon personnalisables  
✅ Sauvegarde du chemin dans un fichier JSON local pour réutilisation ultérieure  
✅ Fenêtre de validation pour enregistrer ou annuler l’opération

## 🖼️ Aperçu

![Démo du script PyRevit](demo.gif)  
📌 *Capture d’écran ou GIF montrant le tracé automatique dans Revit*

## 🛠️ Technologies

- Python 3
- PyRevit
- Autodesk Revit API (version 2025)
- JSON (sauvegarde mémoire)
- Math, GeometryCreationUtilities, TaskDialog

## 📂 Structure du projet

```
📁 /pyrevit-network-optimizer/
├── main_script.py
├── README.md
├── demo.gif
└── memory_paths.json (auto-généré)
```

## 📎 Installation & Usage

1. Ouvrir Revit et lancer PyRevit
2. Charger le script dans un bouton custom via un bundle
3. Suivre les instructions :
   - Sélectionner deux éléments
   - Confirmer l’insertion du conduit
   - Valider l’enregistrement du trajet

> 💡 Nécessite un projet Revit avec un matériau nommé "PVC"

## 🔐 Licence

Ce projet est open-source sous licence MIT. Vous pouvez l'utiliser, le modifier et le partager à condition de mentionner l’auteur.

## 👤 Auteur

**Samuel BROU**  
Étudiant ingénieur à l’ESTP Paris  
Option Jumeaux Numériques & Intelligence Artificielle  
📧 ange.brou@estp.fr  
🔗 [LinkedIn](https://www.linkedin.com/in/ton-lien)

> *Projet développé en collaboration avec l’ESTP Paris*
