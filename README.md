# CareerClarity AI

> Coach de carrière propulsé par l'IA pour salariés en transition et freelances en quête de clarté.

[![Ruby on Rails](https://img.shields.io/badge/Ruby_on_Rails-8.0-CC0000?logo=rubyonrails&logoColor=white)](https://rubyonrails.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Anthropic Claude](https://img.shields.io/badge/Claude_API-D97757?logo=anthropic&logoColor=white)](https://www.anthropic.com/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?logo=bootstrap&logoColor=white)](https://getbootstrap.com/)

---

## Le projet en deux phrases

CareerClarity AI accompagne les personnes qui hésitent dans leurs choix professionnels — reconversion, évolution interne, lancement en freelance — en menant une conversation guidée par un agent IA qui pose les bonnes questions, identifie les leviers et restitue un plan d'action concret.

L'application a été conçue et livrée en équipe de quatre développeurs en **une semaine de sprint**, dans le cadre du parcours **AI Software** du bootcamp Le Wagon (Batch #2208 Marseille, mars 2026).

## Aperçu

> _Captures d'écran à venir._
> _Les screenshots seront ajoutés dès la remise en ligne de la démo._

## Stack technique

| Couche | Choix |
|---|---|
| **Framework** | Ruby on Rails 8 |
| **Base de données** | PostgreSQL |
| **Authentification** | Devise |
| **IA conversationnelle** | RubyLLM + API Anthropic Claude (Sonnet) |
| **Front** | Bootstrap 5, Stimulus, Turbo |
| **Tests** | RSpec, FactoryBot |
| **Déploiement** | Scalingo |
| **CI / collaboration** | Git, GitHub, méthode agile (sprints + revues de code) |

## Fonctionnalités clés

- **Onboarding du parcours** : l'utilisateur décrit sa situation actuelle, ses contraintes et ses aspirations dans un formulaire structuré.
- **Conversation IA contextualisée** : Claude reçoit en entrée le profil et conduit un entretien guidé qui creuse les freins implicites, les ressources mobilisables et les pistes concrètes.
- **Plan d'action restitué** : à la fin de l'entretien, l'IA produit un livrable structuré (forces, alertes, étapes 30/60/90 jours).
- **Historique des sessions** : chaque utilisateur retrouve ses conversations passées et peut reprendre un fil interrompu.
- **Multi-utilisateurs sécurisé** : authentification Devise, séparation stricte des données entre comptes.

## Mon rôle dans l'équipe

Projet collectif à 4 développeurs (aliamzil, Kaliaa77, mariecantau, [Sarah-ABILA](https://github.com/Sarah-ABILA)). J'ai pris en charge **le back-end** en pair-programming, sur les briques suivantes :

### 🗂️ Modélisation & schéma de données
- Conception des modèles **User**, **Session**, **Message** et de leurs relations.
- Migrations Rails et contraintes d'intégrité (clés étrangères, validations).

### 🛣️ Routes & contrôleurs
- Définition des routes RESTful du domaine (sessions de coaching, fil de messages).
- Contrôleurs Rails pour orchestrer la création de session, l'envoi de messages et la restitution du plan d'action.

### 🤖 Intégration Claude API & logique IA
- Branchement de l'**API Anthropic Claude** via la gem **RubyLLM**.
- Construction du **prompt système** spécifique au coaching de carrière.
- Gestion du **contexte de conversation multi-tour** : injection de l'historique et du profil utilisateur dans chaque appel.
- Implémentation de la **logique de plan d'action** restitué en fin d'entretien (forces, alertes, étapes 30/60/90 jours).

### 👥 Méthode
- Pair-programming avec un coéquipier sur les morceaux les plus critiques (intégration IA, contrôleurs).
- Code reviews croisées avec l'ensemble de l'équipe.

> Le repo collaboratif d'origine est [aliamzil/CareerClarity_AI](https://github.com/aliamzil/CareerClarity_AI). Cette version est mon fork personnel pour la mise en avant portfolio. L'historique Git d'origine est conservé.

## Lancer le projet localement

Prérequis : Ruby 3.2+, PostgreSQL 14+, une clé API Anthropic.

```bash
