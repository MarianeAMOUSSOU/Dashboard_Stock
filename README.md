# Dashboard_Stock
# 📊 Dashboard de Gestion de Stock

## 🎯 Contexte
Ce projet Excel illustre la transformation d’un fichier multi-feuilles en un **tableau de bord dynamique** pour piloter la gestion des stocks.  
Il s’appuie sur un modèle pédagogique (entrées, sorties, inventaire, opérations, marchandises) et a été enrichi pour offrir une vue complète de la performance.

---

## 📂 Structure du fichier

### 1. Feuille Marchandises
- Catalogue produit avec :
  - Référence, Désignation, Catégorie, Unité
  - Seuil d’alerte, Stock initial, Prix unitaire, Total
- Formulaire d’ajout de nouvelle marchandise
- Sert de base pour toutes les opérations

### 2. Feuille Opérations
- Interface de saisie des mouvements :
  - Référence, Date, Désignation, Catégorie, Quantité, Prix
- Boutons : `Entrée`, `Sortie`, `Annuler`
- Alimente automatiquement les feuilles **Entrées** et **Sorties**

### 3. Feuille Entrées
- Liste chronologique des approvisionnements :
  - Date, Référence, Désignation, Catégorie, Quantité, Coût, Total
- Permet d’analyser les flux d’entrée et les coûts d’achat

### 4. Feuille Sorties
- Liste des ventes ou retraits :
  - Date, Référence, Désignation, Catégorie, Quantité, Prix de vente, Total
- Sert à calculer la valeur des ventes et analyser la performance

### 5. Feuille Inventaire
- Centralise les données :
  - Stock initial, Entrées, Sorties, Stock final
  - CUMP (Coût Unitaire Moyen Pondéré)
  - Valeur totale
  - Statut (Stock normal, Stock faible, Non disponible)
- Génère des alertes visuelles pour le réapprovisionnement

### 6. Feuille Traitement
- Contient les Tableaux Croisés Dynamiques (TCD) et graphiques construits à partir des données des feuilles "Entrées", "Sorties" et "Inventaire".
- Sert de zone de calcul et d’analyse intermédiaire.
- Alimente le Dashboard en indicateurs et visuels interactifs.

### 7. Feuille Dashboard
- Indicateurs clés :
  - Stock total, Valeur du stock
  - Total des entrées/sorties (quantité + valeur)
- Graphiques :
  - Répartition par catégorie
  - Évolution mensuelle des entrées/sorties
  - Top 3 marchandises
- Alertes :
  - Produits à réapprovisionner
- Filtres interactifs :
  - Mois, Catégorie, Référence

---

## 🧠 Logique globale mise à jour
- **Marchandises** → catalogue produit  
- **Opérations** → formulaire de saisie (non automatisé dans cette version)  
- **Entrées** → historique des approvisionnements  
- **Sorties** → historique des ventes/retraits  
- **Inventaire** → calcul du stock actuel et alertes  
- **Traitement** → TCD + graphiques, base analytique  
- **Dashboard** → synthèse visuelle et dynamique  

---

## ⚠️ Note
Dans cette version, les feuilles **"Opérations"** et **"Marchandises"** servent de modèles de saisie.  
Les scripts VBA pour automatiser l’ajout des entrées/sorties et l’enregistrement des nouvelles marchandises ne sont pas inclus.  
Le projet se concentre sur la création d’un **dashboard interactif et dynamique** pour l’analyse des stocks.  

---

## 🛠️ Technologies utilisées
- Excel (.xlsm) avec macros VBA  
- Tableaux Croisés Dynamiques (TCD)  
- Graphiques dynamiques (barres, courbes, camemberts)  
- Segments (slicers) pour filtrage interactif  
- Mise en forme conditionnelle pour alertes visuelles  
- Formulaires interactifs pour la saisie des opérations

---

## ✨ Résultats
- Pilotage visuel et automatisé de la gestion de stock  
- Saisie simplifiée des opérations  
- Suivi en temps réel des marchandises  
- Détection des ruptures et alertes  
- Export possible en PDF ou présentation  

---

## 🔮 Évolutions possibles
- Automatisation complète des opérations avec VBA  
- Export automatique des rapports en PDF  
- Intégration avec Power BI pour une visualisation avancée  
- Connexion à une base de données SQL pour un suivi en temps réel

---


## 📚 Sources et Remerciements
Le fichier de base utilisé pour ce projet provient d’une formation disponible sur YouTube,  
mise à disposition par la chaîne **Hassan EL BAHI (@hassanbahi)** dans un but pédagogique.  
J’ai suivi cette formation et pratiqué les exercices proposés, puis enrichi le fichier avec mes propres adaptations,  
notamment la mise en place d’un dashboard interactif, de TCD et de graphiques dynamiques,  
ainsi que la documentation complète sur GitHub.  

---

👩‍💻 **Auteur** : Mariane AMOUSSOU  
📅 **Date** : Mars 2026  
📎 **Fichier** : `Dashboard_Stock.xlsm`  
🔗 **Lien GitHub** : https://github.com/MarianeAMOUSSOU/Dashboard_Stock
