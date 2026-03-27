# OrgaRH — Frontend

> Application web de gestion de carrière et des ressources humaines — Interface Angular

[![Angular](https://img.shields.io/badge/Angular-19-red?style=flat-square)](https://angular.io/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue?style=flat-square)](https://www.typescriptlang.org/)
[![PrimeNG](https://img.shields.io/badge/PrimeNG-19-blueviolet?style=flat-square)](https://primeng.org/)
[![Cypress](https://img.shields.io/badge/Tested%20with-Cypress-brightgreen?style=flat-square)](https://www.cypress.io/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)]()

---

## Description

OrgaRH est une application full stack de gestion de carrière développée dans le cadre d'un projet de fin d'études chez **ASSAD Batterie** (Bou Argoub, Tunisie), notée **Excellent**.

Ce dépôt contient le **frontend** : une interface Angular responsive et pixel-perfect, construite avec PrimeNG.

Fonctionnalités principales :
- Interface responsive et multi-navigateurs (pixel-perfect sur tous les appareils)
- Authentification avec formulaire sécurisé (reCAPTCHA intégré)
- Tableau de bord administrateur avec visualisations prédictives
- Gestion des rôles et des accès utilisateurs
- Messagerie interne pour la communication RH
- Tests end-to-end automatisés avec Cypress
- Livraison en sprints Agile/Scrum via Jira

---

## Stack technique

| Couche | Technologie |
|--------|-------------|
| Framework | Angular 17 |
| Langage | TypeScript 5.x |
| UI Components | PrimeNG |
| Styles | CSS3, Design Responsive |
| Tests E2E | Cypress |
| Gestion de projet | Jira, Agile/Scrum |
| Build | Angular CLI |
| Versioning | Git |

---

## Architecture

```
src/
├── app/
│   ├── core/              # Guards, interceptors, services globaux
│   ├── shared/            # Composants réutilisables, pipes
│   ├── features/
│   │   ├── auth/          # Login, register, reCAPTCHA
│   │   ├── dashboard/     # Tableau de bord admin
│   │   ├── employes/      # Gestion des employés
│   │   ├── carrieres/     # Suivi de carrière
│   │   └── messagerie/    # Messagerie interne RH
│   └── app-routing.module.ts
├── assets/
├── environments/
│   └── environment.example.ts
└── cypress/
    └── e2e/               # Tests automatisés
```

---

## Prérequis

- Node.js 18+
- npm 9+
- Angular CLI 17+
- Backend OrgaRH en cours d'exécution sur `http://localhost:9090`

---

## Installation

### 1. Cloner le dépôt

```bash
git clone https://github.com/TON_USERNAME/orgarh-frontend.git
cd orgarh-frontend
```

### 2. Installer les dépendances

```bash
npm install
```

### 3. Configurer l'environnement

Copier le fichier exemple :

```bash
cp src/environments/environment.example.ts src/environments/environment.ts
```

Vérifier que l'URL du backend est correcte :

```typescript
export const environment = {
  production: false,
  apiUrl: 'http://localhost:9090'
};
```

### 4. Lancer l'application

```bash
ng serve
```

L'interface sera disponible sur `http://localhost:4200`

---

## Tests

Lancer les tests end-to-end Cypress :

```bash
npx cypress open
```

Ou en mode headless :

```bash
npx cypress run
```

---

## Backend

L'API REST Spring Boot de ce projet est disponible ici :
**[orgarh-backend](https://github.com/TON_USERNAME/orgarh-backend)**

---

## Auteure

**Mariem Jlassi**
Étudiante Ingénieure en Informatique — iTeam University, Tunis

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mariem%20Jlassi-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/mariem-jlassi)
[![Portfolio](https://img.shields.io/badge/Portfolio-mariem--portfolio.netlify.app-orange?style=flat-square)](https://mariem-portfolio.netlify.app)

---

*Projet de Fin d'Études — Février 2025 à Mai 2025 — Note : Excellent*
