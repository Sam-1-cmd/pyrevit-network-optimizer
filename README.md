# pyrevit-network-optimizer

# 🛠️ Génération intelligente de conduits dans Revit avec PyRevit

🎓 Projet réalisé dans le cadre de ma formation à l’ESTP Paris, option Jumeaux Numériques et Intelligence Artificielle.

## 🎯 Objectif

Outil PyRevit conçu pour automatiser le tracé de conduits dans Revit, avec détection d’obstacles et génération d’un chemin contourné entre deux éléments.
L’objectif est de faciliter la modélisation des réseaux techniques en prenant en compte les obstacles présents dans le modèle (murs, poutres, etc.) et en générant un trajet optimisé pour le passage du conduit.

## ⚙️ Fonctionnalités

| Fonction | Description |
|----------|-------------|
| 🧩 Sélection | Deux éléments MEP sélectionnés dans Revit |
| 📍 Calcul des centres | Revit API utilisée pour récupérer les coordonnées |
| 🚧 Obstacles | Détection via `ReferenceIntersector` |
| 🔁 Contournement | Génération automatique de points intermédiaires |
| 📐 Conduits | Modélisation 3D avec matériau et rayon personnalisables |
| 💾 Mémoire | Fichier JSON utilisé pour stocker les trajets |
| ✅ Validation | Interface utilisateur pour confirmer ou annuler l’action |


## 🖼️ Aperçu

![Démo du script PyRevit](demo.gif)  
*GIF montrant le tracé automatique dans Revit*

## 🛠️ Technologies

- Python 
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
Parcours en Transition Numérique de la construction
Option Jumeaux Numériques & Intelligence Artificielle  
📧 ange.brou@estp.fr  
🔗 [LinkedIn](https://www.linkedin.com/in/brou-ange-samuel-8945442aa?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BjVq%2FbBG2SpG6xsyqPbvaPw%3D%3D)

> *Projet développé en collaboration avec l’ESTP Paris*
