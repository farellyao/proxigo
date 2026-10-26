# ProxiGo — frontend connecté à Supabase

Cette application React/Vite utilise le projet Supabase ProxiGo existant.

## Lancer
1. Installer Node.js 20+.
2. Copier `.env.example` vers `.env.local`.
3. `npm install`
4. `npm run dev`
5. Ouvrir l’URL locale affichée par Vite.

## Fonctions présentes
- Authentification e-mail/mot de passe Supabase.
- Lecture des boutiques actives et des produits disponibles.
- Demande de création de boutique en attente de validation.
- Ajout de produits au catalogue d’une boutique possédée.
- Panier limité à une boutique et enregistrement des commandes + lignes dans PostgreSQL.
- Liste des commandes du compte connecté.

## Avant la production
Tester chaque parcours avec plusieurs comptes et les politiques RLS. L’administration de validation, les notifications temps réel, les photos, le suivi GPS et Mobile Money restent à développer. Le frontend utilise uniquement une clé publishable ; ne jamais y mettre une clé service_role.
