# 🪐 ORBITE by Kweb

> **Apprends. Évolue. Trouve ton orbite.**

ORBITE by Kweb est une plateforme d'apprentissage en ligne nouvelle génération qui combine **formations vidéo, parcours pédagogiques, intelligence artificielle et apprentissage adaptatif**.

L'objectif n'est pas simplement de vendre des cours. ORBITE doit accompagner chaque apprenant depuis la définition de son objectif jusqu'à la maîtrise progressive des compétences nécessaires pour l'atteindre.

---

## ✨ Vision

ORBITE place l'apprenant au centre de son propre système d'apprentissage.

Le parcours cible est :

```text
Objectif
   ↓
Diagnostic
   ↓
Parcours personnalisé
   ↓
Formation
   ↓
Accompagnement IA
   ↓
Exercices
   ↓
Évaluation
   ↓
Adaptation
   ↓
Progression
   ↓
Certification
```

Le concept d'**orbite** représente les objectifs, les compétences, les formations, les agents IA et les différentes étapes de progression qui gravitent autour de l'apprenant.

---

## 🎯 Proposition de valeur

ORBITE vise à réunir dans une seule expérience :

- 🎓 des formations vidéo structurées ;
- 🧠 des agents IA spécialisés comme formateurs et assistants ;
- 🪐 des parcours d'apprentissage personnalisés ;
- 📈 une progression basée sur les compétences ;
- 📝 des exercices et évaluations ;
- 🔄 une adaptation du parcours selon les résultats ;
- 👨‍🏫 un espace formateur ;
- 🤖 une création de formations assistée par IA ;
- 🏆 des certificats ;
- 🛒 une marketplace de formations ;
- 💳 une architecture de paiement extensible ;
- 📊 des outils d'analyse et de suivi.

---

## 🤖 ORBITE AI

L'intelligence artificielle est une partie centrale du produit, mais ORBITE AI n'est pas conçu comme un simple chatbot.

Le système doit fonctionner comme un ensemble d'agents spécialisés orchestrés par le backend.

### Agents envisagés

| Agent | Domaine / responsabilité |
|---|---|
| **KODEX** | Programmation et ingénierie logicielle |
| **KORA** | Marketing, communication et réseaux sociaux |
| **NOVA** | Business, entrepreneuriat et stratégie |
| **PIXEL** | Design et créativité |
| **LUMEN** | Sciences, mathématiques et raisonnement analytique |
| **AURA** | Développement personnel, productivité et méthodologie d'apprentissage |

La liste des agents pourra évoluer avec le produit.

### Architecture IA cible

```text
Utilisateur
    ↓
Django API
    ↓
AI Orchestrator
    ↓
Context Builder
    ↓
Agent spécialisé
    ↓
Tools / Knowledge / RAG
    ↓
LLM
    ↓
Validation
    ↓
Django
    ↓
Utilisateur
```

Les agents ne doivent pas disposer d'un accès arbitraire à la base de données. Ils doivent utiliser des outils et services contrôlés par le backend.

---

## 🧠 Apprentissage adaptatif

L'une des fonctionnalités différenciantes d'ORBITE est son futur **Learning Engine**.

Le moteur pourra prendre en compte :

- l'objectif de l'apprenant ;
- son niveau initial ;
- ses compétences ;
- ses résultats ;
- ses erreurs ;
- sa progression ;
- son historique ;
- son temps disponible ;
- ses préférences pédagogiques.

Il pourra ensuite recommander :

- la prochaine leçon ;
- une révision ;
- un exercice ;
- un quiz ;
- une difficulté différente ;
- une ressource complémentaire ;
- une modification du parcours.

### Exemple

```text
Compétence Python       89%
Django                  62%
APIs                    41%
Dernier quiz            55%

          ↓

ORBITE recommande :

1. Révision HTTP
2. Exercice API niveau débutant
3. Nouvelle évaluation
4. Passage au module suivant si maîtrise suffisante
```

Les recommandations IA doivent rester séparées des règles métier et des données de référence.

---

## 👨‍🏫 Formateurs humains + IA

ORBITE doit également permettre aux formateurs de créer et publier leurs propres formations.

L'IA pourra assister le formateur dans :

- la conception du programme ;
- la structuration des modules ;
- la génération d'idées d'exercices ;
- la création de quiz ;
- la génération de supports complémentaires ;
- l'analyse pédagogique ;
- l'amélioration du parcours.

### Principe important

```text
IA propose
   ↓
Formateur vérifie
   ↓
Formateur modifie
   ↓
Formateur valide
   ↓
Publication
```

Une formation générée ou enrichie par IA ne doit pas être publiée automatiquement sans validation humaine lorsque le produit exige cette validation.

---

## 👥 Types d'utilisateurs

### Apprenant

Peut notamment :

- créer un compte ;
- définir ses objectifs ;
- découvrir des formations ;
- acheter des formations ;
- suivre des cours ;
- interagir avec les agents IA ;
- réaliser des exercices ;
- passer des évaluations ;
- suivre ses compétences ;
- consulter sa progression ;
- obtenir des certificats.

### Formateur

Peut notamment :

- créer une formation ;
- organiser ses modules ;
- ajouter des vidéos et ressources ;
- créer des évaluations ;
- utiliser l'assistance IA ;
- gérer ses formations ;
- suivre les apprenants selon les fonctionnalités prévues ;
- publier et gérer son contenu.

### Administrateur

Peut notamment :

- gérer les utilisateurs ;
- gérer les formations ;
- modérer les contenus ;
- gérer les catégories ;
- superviser les commandes ;
- superviser les paiements ;
- gérer les agents IA ;
- consulter les analytics ;
- administrer la plateforme.

---

## 🧩 Modules fonctionnels

L'architecture fonctionnelle cible comprend notamment :

```text
ORBITE
├── Authentification
├── Utilisateurs / Profils
├── Catalogue
├── Formations
├── Modules / Leçons
├── Lecteur vidéo
├── Parcours d'apprentissage
├── Objectifs
├── Compétences
├── Progression
├── Exercices
├── Quiz / Évaluations
├── ORBITE AI
├── Learning Engine
├── Espace Formateur
├── Création assistée par IA
├── Panier
├── Commandes
├── Paiements
├── Certificats
├── Notifications
├── Reviews
├── Analytics
└── Administration
```

---

## 🏗️ Architecture technique

ORBITE est conçu autour d'une architecture **Django + React API-first**.

```text
                         ORBITE
                            │
          ┌─────────────────┴─────────────────┐
          │                                   │
       React                               Django
      Frontend                           Backend API
          │                                   │
          │                       ┌───────────┼───────────┐
          │                       │           │           │
          │                    Learning    Commerce      Users
          │                       │           │           │
          │                       └─────┬─────┴───────────┘
          │                             │
          │                         ORBITE AI
          │                             │
          │                  ┌──────────┼──────────┐
          │                  │          │          │
          │                Tutor     Adaptive    Builder
          │                  │         Engine        │
          │                  └──────────┼───────────┘
          │                             │
          └─────────────────────────────┤
                                        ↓
                                   PostgreSQL
                                        │
                                Redis / Celery
                                        │
                               File / Video Storage
```

---

## 🐍 Backend

### Stack cible

- **Python**
- **Django**
- **Django REST Framework**
- **PostgreSQL**
- **Redis**
- **Celery**

### Responsabilités

Django est la **source de vérité** de l'application.

Il gère notamment :

- authentification ;
- utilisateurs ;
- permissions ;
- formations ;
- progression ;
- évaluations ;
- compétences ;
- commandes ;
- paiements ;
- certificats ;
- IA ;
- notifications ;
- analytics.

---

## ⚛️ Frontend

### Stack cible

- **React**
- **Vite**
- **Tailwind CSS**

Le frontend est responsable de l'expérience utilisateur et consomme l'API REST Django.

Organisation fonctionnelle envisagée :

```text
frontend/
└── src/
    ├── components/
    ├── layouts/
    ├── pages/
    ├── features/
    │   ├── auth/
    │   ├── courses/
    │   ├── learning/
    │   ├── ai/
    │   ├── progress/
    │   ├── certificates/
    │   ├── cart/
    │   └── checkout/
    ├── hooks/
    ├── services/
    ├── store/
    ├── routes/
    └── utils/
```

Cette structure est une direction d'architecture et pourra être ajustée lors de l'implémentation réelle.

---

## 🗄️ Données principales

Les principales entités envisagées sont :

```text
User
Profile
Role
Course
Category
Module
Lesson
Video
Resource
Skill
UserSkill
Enrollment
LessonProgress
Quiz
Question
Attempt
Exercise
Submission
LearningPath
Goal
Recommendation
AIAgent
AISession
AIMessage
AIMemory
AIContext
Order
OrderItem
Payment
PaymentTransaction
Certificate
Notification
Review
AnalyticsEvent
```

Le modèle de données définitif devra être validé avant une implémentation complète.

---

## 🔌 API

L'API est prévue sous :

```text
/api/v1/
```

Domaines principaux :

```text
/api/v1/auth/
/api/v1/users/
/api/v1/courses/
/api/v1/learning/
/api/v1/skills/
/api/v1/assessments/
/api/v1/exercises/
/api/v1/ai/
/api/v1/cart/
/api/v1/orders/
/api/v1/payments/
/api/v1/certificates/
/api/v1/notifications/
/api/v1/analytics/
```

Les contrats API détaillés seront définis avant les implémentations correspondantes.

---

## 💳 Paiements

ORBITE doit utiliser une architecture de paiement abstraite afin de pouvoir intégrer plusieurs moyens de paiement.

Le premier moyen envisagé est **Orange Money**, avec un fonctionnement semi-automatique dans une phase ultérieure.

Architecture cible :

```text
Order
  ↓
Payment Service
  ↓
Payment Provider
  ↓
Transaction
  ↓
Verification
  ↓
Order confirmation
  ↓
Enrollment / Access
```

**Important :** les détails techniques d'Orange Money ne sont pas considérés comme définitifs dans ce dépôt tant qu'ils n'ont pas été validés pour la phase d'implémentation.

Le frontend ne doit jamais être la source de vérité pour l'état d'un paiement.

---

## 🔐 Sécurité

Principes fondamentaux :

- HTTPS en production ;
- secrets dans les variables d'environnement ;
- permissions contrôlées côté backend ;
- validation stricte des données ;
- CORS correctement configuré ;
- protection CSRF selon l'architecture d'authentification ;
- rate limiting sur les endpoints sensibles ;
- contrôle des accès aux contenus ;
- protection des fichiers et vidéos ;
- isolation des outils IA ;
- journalisation des actions sensibles ;
- aucune clé secrète dans React ;
- aucune confiance dans les données sensibles envoyées par le frontend.

---

## 🎨 Identité visuelle

ORBITE adopte une direction **minimaliste, premium, technologique et immersive**.

### Palette

| Usage | Couleur |
|---|---|
| Obsidienne | `#08090D` |
| Surface | `#11131A` |
| Violet Orbite | `#7C5CFF` |
| Cyan | `#22D3EE` |
| Succès | `#34D399` |
| Texte principal | `#F8FAFC` |
| Texte secondaire | `#94A3B8` |

### Typographie

- **Space Grotesk** — titres et identité
- **Inter** — interface et contenu

### Principes

- simplicité avant décoration ;
- animations fonctionnelles ;
- espace visuel généreux ;
- glow subtil ;
- excellente lisibilité ;
- expérience mobile prioritaire ;
- identité orbitale cohérente.

Le symbole ORBITE doit pouvoir fonctionner indépendamment du wordmark.

---

## 🪐 Concept d'interface

L'expérience utilisateur doit être centrée sur l'idée :

> **Le centre = l'apprenant. Les orbites = son évolution.**

La progression pourra être représentée par des compétences et objectifs gravitant autour d'un noyau central.

L'interface ne doit cependant pas devenir une visualisation complexe au détriment de la lisibilité.

---

## 📱 Expérience mobile

Le mobile est considéré comme une expérience principale.

Navigation cible :

```text
Accueil
Cours
Orbite
IA
Profil
```

Le lecteur vidéo, les exercices et l'interaction avec l'IA doivent être particulièrement adaptés aux écrans mobiles.

---

## 🧪 Qualité et tests

Le projet devra progressivement intégrer :

- tests unitaires backend ;
- tests API ;
- tests des permissions ;
- tests frontend ;
- tests des parcours utilisateurs ;
- tests des paiements ;
- tests des flux IA ;
- tests de sécurité ;
- tests end-to-end.

Aucune fonctionnalité critique ne doit être considérée comme terminée uniquement parce que son interface fonctionne.

---

## 🗺️ Roadmap indicative

### Phase 0 — Fondations

- architecture du projet ;
- configuration Django ;
- configuration React ;
- base PostgreSQL ;
- authentification ;
- structure API ;
- design system.

### Phase 1 — MVP

- utilisateurs ;
- catalogue ;
- formations ;
- modules et leçons ;
- lecteur vidéo ;
- progression ;
- panier ;
- commandes ;
- première gestion des accès.

### Phase 2 — Commerce

- paiements ;
- intégration Orange Money ;
- vérification des transactions ;
- notifications ;
- gestion commerciale.

### Phase 3 — ORBITE AI

- AI Orchestrator ;
- agents spécialisés ;
- assistant de cours ;
- contexte pédagogique ;
- génération d'exercices ;
- première couche de recommandations.

### Phase 4 — Learning Engine

- compétences ;
- diagnostic ;
- mastery score ;
- parcours adaptatifs ;
- recommandations avancées ;
- personnalisation pédagogique.

### Phase 5 — Écosystème formateur

- espace formateur avancé ;
- Course Builder AI ;
- génération assistée de parcours ;
- exercices et évaluations assistés par IA ;
- outils de publication et de gestion.

### Phase 6 — Évolution avancée

- analytics avancés ;
- nouvelles familles d'agents ;
- nouvelles méthodes pédagogiques ;
- nouvelles intégrations ;
- expansion internationale.

---

## 🚧 Statut du projet

**Statut : 🟡 En développement — phase de fondation**

Le dépôt constitue le point de départ technique du développement d'ORBITE by Kweb.

Les fonctionnalités et architectures décrites ici représentent la vision et la spécification actuelle du produit. Elles seront affinées au fur et à mesure de l'implémentation.

---

## 📚 Documentation projet

La documentation détaillée du projet doit couvrir progressivement :

- cahier des charges ;
- architecture fonctionnelle ;
- architecture technique ;
- modèle de données ;
- contrats API ;
- architecture des agents IA ;
- learning engine ;
- design system ;
- sécurité ;
- stratégie de tests ;
- déploiement ;
- roadmap ;
- décisions techniques.

La documentation détaillée constitue la référence avant toute décision d'implémentation importante.

---

## 🤝 Principes de développement

### Backend first as source of truth

Le backend valide les permissions, les achats, les accès, la progression et les opérations sensibles.

### AI with controlled capabilities

Les agents IA utilisent des outils contrôlés plutôt qu'un accès direct et illimité aux données internes.

### Modular architecture

Chaque domaine fonctionnel doit pouvoir évoluer sans casser l'ensemble de la plateforme.

### API-first

Les contrats entre React et Django doivent être explicites et versionnés.

### Learning-first UX

Chaque écran doit aider l'utilisateur à comprendre ce qu'il doit faire ensuite.

### Human validation where needed

L'IA assiste les apprenants et les formateurs, mais certaines décisions ou publications doivent rester sous contrôle humain.

---

## 🔭 Vision long terme

ORBITE peut évoluer progressivement d'une plateforme de formations vers une infrastructure d'apprentissage personnalisée :

```text
Plateforme de formations
        ↓
Formations + IA
        ↓
Apprentissage adaptatif
        ↓
Création de formations assistée par IA
        ↓
Écosystème pédagogique intelligent
        ↓
Personal Learning OS
```

L'ambition est de construire une expérience dans laquelle l'apprenant ne reçoit pas simplement du contenu : **le système comprend son objectif, observe sa progression et l'aide à avancer vers la maîtrise.**

---

## 🏷️ Branding

**ORBITE**  
*by Kweb*

> **Apprends. Évolue. Trouve ton orbite.**

---

## 📄 Licence

La licence du projet et les conditions de distribution seront définies ultérieurement.
