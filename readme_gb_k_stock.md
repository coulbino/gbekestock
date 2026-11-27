# GbêkêStock — Gestion de Stock pour Commerçants de Bouaké

**GbêkêStock** est une application web légère de gestion d'inventaire en temps réel, conçue pour simplifier le suivi des marchandises, des ventes au comptoir et des alertes de rupture de stock pour les commerçants de Bouaké (Marché Central, Koko, Air France, Dar-es-Salam).

---

## Fonctionnalités principales

- **Tableau de bord en temps réel :**
  - Compteur dynamique du nombre total de références et d'unités en magasin.
  - Calcul automatique de la valorisation totale du stock en **FCFA**.
  - Alerte visuelle immédiate sur le nombre de produits en rupture de stock.
- **Enregistrement rapide des arrivages :** Ajout de nouveaux articles (nom, quantité, prix unitaire en FCFA) avec mise à jour instantanée de l'inventaire.
- **Vente au comptoir en un clic :** Bouton **« Vendre 1 article »** décrémentant le stock en direct avec notifications *toast* (confirmation de vente ou alerte de rupture).
- **Recherche instantanée :** Filtrage rapide des marchandises par nom d'article.
- **Indicateurs visuels d'état :** Badges colorés distinguant les articles en stock, en stock faible ($\le 3$ unités) ou en rupture ($0$ unité).

---

## Technologies utilisées

- **HTML5** (structure sémantique accessible)
- **Tailwind CSS** (via CDN, design responsive mobile et ordinateur)
- **JavaScript Vanilla (ES6+)** (gestion de l'état, calculs en temps réel, rendu dynamique du DOM et protection XSS)
- **Google Fonts (Inter)**

---

## Lancement du projet en local

Aucune installation de serveur ou de dépendance n'est requise :

1. Clonez ce dépôt ou téléchargez le fichier `index.html` :
   ```bash
   git clone https://github.com/coulbino/gbekestock.git
   ```
2. Ouvrez simplement le fichier `index.html` dans n'importe quel navigateur web moderne (Chrome, Edge, Firefox).

---

## Architecture et évolutions prévues

Ce prototype a été volontairement conçu sous forme d'application autonome monofichier (`index.html`) afin de garantir un déploiement immédiat et une exécution sans configuration.

**Prochaines étapes d'amélioration :**
- **Découpage modulaire :** Séparation du code en fichiers distincts (`index.html`, `style.css`, `app.js`).
- **Persistance des données :** Sauvegarde locale via `localStorage` ou connexion à une base de données (MySQL / Supabase) pour conserver l'inventaire entre deux sessions.
- **Historique des ventes :** Export journalier des ventes et des mouvements de stock.

---

## Auteur

Développé par **Kolotcholoma Coulibaly** (`coulbino`) — Étudiant en Licence 3 Informatique (Spécialisation Bases de Données & Génie Logiciel).