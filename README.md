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

Projet collectif à 4 développeurs (aliamzil, Kaliaa77, mariecantau, [Sarah-ABILA](https://github.com/Sarah-ABILA)). Mes contributions principales :

- Conception du schéma de données (utilisateurs, sessions, messages).
- Intégration de l'API Anthropic via RubyLLM, gestion du contexte de conversation côté serveur.
- Pages Devise + flux d'onboarding (formulaires Stimulus).
- Code reviews croisées avec l'équipe.

> Le repo collaboratif d'origine est [aliamzil/CareerClarity_AI](https://github.com/aliamzil/CareerClarity_AI). Cette version est mon fork personnel pour la mise en avant portfolio. L'historique Git d'origine est conservé.

## Lancer le projet localement

Prérequis : Ruby 3.2+, PostgreSQL 14+, une clé API Anthropic.

```bash
git clone https://github.com/Sarah-ABILA/CareerClarity_AI.git
cd CareerClarity_AI

bundle install
yarn install

# Configurer les variables d'environnement
cp .env.example .env
# Éditer .env et renseigner ANTHROPIC_API_KEY=sk-...

# Préparer la base
rails db:create db:migrate db:seed

# Démarrer
bin/dev
```

L'application est disponible sur `http://localhost:3000`.

## Ce que j'ai appris sur ce projet

- Travailler en sprint Agile très court (1 semaine) sur un produit livrable de bout en bout.
- Concevoir un prompt système robuste pour un agent IA conversationnel multi-tour.
- Découper un produit complexe en tickets actionnables et les livrer en revue de code.
- Gérer les conflits de merge et la coordination Git à 4.

## Ressources

- [Démarche pédagogique Le Wagon AI Software](https://www.lewagon.com/fr/data-science-course)
- [Anthropic Claude API documentation](https://docs.anthropic.com/)
- [RubyLLM gem](https://github.com/crmne/ruby_llm)

---

_Sarah Abila — Hyères (83) — [LinkedIn](https://linkedin.com/in/sarah-abila-278041378) — [GitHub](https://github.com/Sarah-ABILA)_
