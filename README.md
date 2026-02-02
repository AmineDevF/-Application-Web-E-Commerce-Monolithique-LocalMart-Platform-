## Application Web E-Commerce Monolithique (LocalMart)

## Contexte

Afin de faciliter l’accès aux produits du quotidien et de soutenir le commerce local, l’entreprise **LocalMart** souhaite mettre en place une plateforme de boutique en ligne centralisée.

Cette application permettra à des vendeurs de proposer leurs produits, tandis que les clients pourront consulter le catalogue, passer des commandes, suivre leur statut et interagir avec les produits (likes, avis).

Le projet a pour objectif de simuler un véritable écosystème e-commerce, tout en mettant l’accent sur :

- Une architecture monolithique Laravel scalable
- La gestion des rôles et permissions
- L’utilisation des middlewares et policies
- Les notifications
- Les relations avancées entre entités

---

## Objectifs du Projet

Concevoir et développer une application web monolithique avec Laravel permettant :

- La gestion des utilisateurs avec authentification et autorisation
- La vente de produits avec gestion des stocks
- La gestion complète du cycle de vie d’une commande
- L’envoi de notifications email aux utilisateurs
- L’application de règles métiers via middleware et policies

### Bonus

- Intégration du paiement en ligne
- Notifications en temps réel

L’application devra être **sécurisée**, **documentée** et **déployée sur un environnement Linux**.

---

## Fonctionnalités Clés

### Boutique en Ligne

- Catalogue de produits avec catégories
- Page détail produit (description, prix, stock, avis)
- Gestion des stocks en temps réel

### Panier et Commandes

- Ajout et suppression de produits au panier
- Validation de commande
- Suivi du statut de commande :
  - En attente
  - Payée
  - Livrée

### Authentification et Autorisation

- Authentification avec Laravel Breeze ou Jetstream
- Gestion multi-rôles via Spatie Laravel Permission :
  - Client
  - Seller
  - Admin
  - Moderator
- Protection des routes par middleware
- Gestion des autorisations via policies

### Interactions Utilisateur

- Like sur les produits
- Système de notation
- Avis et commentaires

### Notifications

Notifications email (Gmail) lors :

- D’une nouvelle commande
- D’un changement de statut de commande
- D’un nouvel avis sur un produit

### Paiement en Ligne (Bonus)

- Intégration d’un seul moyen de paiement :
  - Stripe ou Mollie
- Gestion du statut de paiement
- Utilisation des webhooks

### Temps Réel (Bonus)

- Notifications instantanées avec Laravel Reverb ou Pusher
- Mise à jour en direct :
  - Du statut des commandes
  - Des likes et avis

---

## Technologies Requises

- Framework backend : Laravel (11)
- Frontend : Blade + Tailwind CSS
- Base de données : MySQL ou PostgreSQL
- Authentification : Laravel Breeze ou Jetstream
- Rôles et permissions : Spatie Laravel Permission
- Paiement (Bonus) : Stripe ou Mollie
- Temps réel (Bonus) : Laravel Reverb ou Pusher
- Versioning : Git et GitHub
- Déploiement on render : (opptionnel) 

---

## User Stories

### Rôle : Client

- En tant que client, je peux créer un compte et me connecter à la plateforme
- En tant que client, je peux consulter le catalogue des produits par catégorie
- En tant que client, je peux ajouter des produits à mon panier
- En tant que client, je peux passer une commande
- En tant que client, je peux suivre le statut de ma commande
- En tant que client, je peux liker et noter un produit
- En tant que client, je reçois une notification email lors d’un changement de statut

### Rôle : Seller

- En tant que vendeur, je peux créer, modifier et supprimer mes produits
- En tant que vendeur, je peux définir le prix et le stock de mes produits
- En tant que vendeur, je reçois une notification lors d’une nouvelle commande
- En tant que vendeur, je peux mettre à jour le statut d’une commande

### Rôle : Administrateur

- En tant qu’administrateur, je peux gérer les utilisateurs et leurs rôles
- En tant qu’administrateur, je peux modérer les produits et les avis
- En tant qu’administrateur, je peux consulter l’ensemble des commandes
- En tant qu’administrateur, je peux accéder à une vue globale des statistiques

### Rôle : Moderator

- En tant que modérateur, je peux supprimer ou masquer des avis inappropriés
- En tant que modérateur, je peux suspendre temporairement un utilisateur ou un produit

---

## Livrables Attendus

- Code source versionné sur GitHub
- Base de données structurée et documentée
- Documentation technique du projet
- Application fonctionnelle déployée sur Linux

---

