# BNC 360

Preuve de concept d'une plateforme de pilotage interne pour le Bureau National de la CEDEAO en Côte d'Ivoire.

**Démonstration en ligne :** https://ferie-acs.github.io/bnc-360/

## Périmètre fonctionnel

| Domaine | Modules |
|---|---|
| Pilotage | Vue 360°, indicateurs, projets (cadre logique, plan d'action, jalons, financements, risques), instructions, point hebdomadaire |
| Mission CEDEAO | Textes communautaires, points focaux, signalements, événements, réunions statutaires |
| Administration | Courrier, réunions et comptes rendus (émargement par QR code), missions, personnel, arrivées et départs, budget, agenda |
| Ressources | Documents, partenaires, logistique, visiteurs |
| Système | Comptes et accès, notifications, règles et paramètres, journal d'audit |

## Règles automatiques

- Échéances du courrier calculées en jours ouvrés (week-ends et jours fériés exclus), routage par catégorie et suppléance en cas d'absence.
- Escalade paramétrable : rappel à l'agent, alerte au chef de service, remontée au Coordonnateur.
- Contrôle des congés : solde, taux d'absents par service, périodes réservées, intérim obligatoire en présence d'un jalon.
- Parcours d'intégration et procédure de départ avec échéances calculées, passation des dossiers et fermeture des accès.
- Politique de mots de passe, verrouillage, double authentification et revue périodique des accès.
- Traçabilité de chaque action au journal d'audit.

## Profils de démonstration

Le sélecteur de profil, en haut à droite, permet de basculer entre : Coordonnateur, Secrétaire de Direction, Chargée de programmes, Administrateur de la plateforme.

## Notes techniques

- Application monopage en HTML, CSS et JavaScript, sans serveur ni dépendance de compilation.
- Les données sont fictives et conservées dans le navigateur (localStorage) ; les envois d'e-mails et de SMS sont simulés.
- Bibliothèques chargées depuis un CDN : Lucide (icônes) et qrcode-generator.

## Statut

Preuve de concept — octobre 2026. Les valeurs de paramétrage (délais, barèmes, politique de sécurité) sont des valeurs de démonstration à confirmer.
