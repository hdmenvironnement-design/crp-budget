# CRP — Gestion de budget

Prototype de gestion budgétaire en français, conçu pour ordinateur et Android sous forme de PWA.

## Fonctionnalités présentes
- Tableau de bord par mois, solde estimé et répartition des dépenses
- Ajout de revenus, dépenses et virements/épargne
- Catégories et plafonds budgétaires personnalisables
- Dépenses récurrentes avec action pour les enregistrer
- Objectifs d'épargne
- Suivi des crédits et remboursements
- Recherche et filtre des opérations
- Export des opérations en CSV et sauvegarde/restauration JSON
- Mise en cache PWA pour une ouverture hors ligne après le premier chargement

## Démarrage local
Ouvrir `index.html` permet de tester l'interface, mais certaines fonctions PWA nécessitent un serveur HTTPS ou localhost.

Pour servir le dossier avec Python :
```bash
python -m http.server 8000
```
Puis ouvrir `http://localhost:8000`.

## Installation sur Android
1. Publier le dossier sur un hébergement HTTPS.
2. Ouvrir l'adresse dans Chrome sur Android.
3. Menu ⋮ > Installer l'application (ou Ajouter à l'écran d'accueil).

## Synchronisation entre appareils — importante
Cette version enregistre les données dans le stockage local du navigateur. Elle **ne synchronise pas encore** automatiquement téléphone et ordinateur. Pour une vraie synchronisation multi-appareils, il faut ajouter une authentification, une base de données distante, des règles d'accès strictes et un hébergement (par exemple Supabase ou Firebase), puis publier le site en HTTPS.

Ne stockez pas de mots de passe bancaires dans cette application. L'import de relevés bancaires et les connexions bancaires ne sont pas implémentés.
