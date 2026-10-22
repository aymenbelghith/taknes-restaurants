# Andaluz Restaurant — prototype premium

**Identité de la démonstration** : Andaluz Restaurant · Cuisine halal · Élancourt 78990 · tous les jours de 10 h à 22 h · téléphone/WhatsApp 06 43 86 66 38.

## Lancer le site

Ouvrir `index.html` dans un navigateur moderne, ou lancer un serveur local dans ce dossier :

```bash
python -m http.server 8000
```

Puis accéder à http://localhost:8000.

## Fonctionnalités interactives

- Site responsive, carte filtrable et fiches produit avec suppléments.
- Panier avec quantités, code promo **ANDALUZ10** (fictif), choix de retrait et confirmation locale.
- Conseiller de menu simulé : recommandations calculées selon un budget, une préférence et la faim. **Il n'utilise pas une API d'intelligence artificielle.**
- Espace restaurateur **de démonstration**, accessible dans le pied de page : commandes locales, changement de statut, disponibilités et prix de démonstration.
- Boutons WhatsApp et téléphone, lien Google Maps dirigé vers la commune d'Élancourt (pas une adresse de restaurant).

## Important avant toute utilisation réelle

**Ce projet est un prototype front-end et non une plateforme de commandes opérationnelle.** Les commandes sont stockées seulement dans `localStorage` sur le navigateur utilisé : elles ne sont envoyées à aucun restaurateur et ne sont pas synchronisées entre appareils. L'espace restaurateur n'a aucune authentification et ne doit pas être exposé comme un back-office sécurisé en production.

À développer/configurer pour une mise en service :

1. Serveur, base de données, API de commande et mises à jour en temps réel, contrôle des capacités et authentification du restaurateur.
2. Hébergement HTTPS, domaine, informations légales, RGPD (y compris données des commandes), politiques de cookies, confidentialité et sécurité.
3. Vraie adresse, tarifs, descriptions, images des plats, menus, disponibilité, allergènes, éventuelle certification halal et liens réseaux sociaux validés par le restaurateur. Tous les prix actuels sont indicatifs.
4. Paiement en ligne seulement si demandé, via un prestataire adapté.
5. API IA côté serveur si un véritable assistant conversationnel IA est souhaité ; la version présente est une suggestion algorithmique locale.

## Personnalisation

La carte initiale et ses prix se trouvent dans `app.js`, dans la constante `menu`. Les textes et le numéro sont dans `index.html`. Les photos sont dans `assets`.

Visuels des aliments générés par IA : photos conceptuelles, non contractuelles. La photo de boissons en canettes est recadrée d'une maquette générée par IA ; elle sert uniquement à illustrer les boissons emballées.
