# BAYA - Plateforme de Santé Numérique

**Tagline:** "Parce que chaque battement compte."

## 🎯 Vue d'ensemble

BAYA est une plateforme complète de santé numérique conçue pour le suivi des grossesses et la santé maternelle. Elle offre une expérience multi-rôles pour les femmes enceintes, les sages-femmes, les gynécologues, les agents communautaires et les proches.

## 🎨 Design System

### Couleurs BAYA
- **Violet principal:** `#6D3EF7` (260°, 84%, 50% HSL)
- **Rose maternité:** `#F857A6` (330°, 85%, 60% HSL)
- **Vert santé:** `#1DB954` (120°, 60%, 50% HSL)
- **Bleu médical:** `#2F80ED` (Blue accent)

### Alertes de santé
- **Vert:** Normal - État normal
- **Jaune:** Surveillance - À surveiller
- **Orange:** Consultation - Consultation recommandée
- **Rouge:** Urgence - Action immédiate requise

### Typographie
- **Headings:** Poppins (500, 600, 700, 800)
- **Body text:** Inter (400, 500, 600, 700)

### Composants
- Boutons arrondis (16-20px)
- Ombres douces
- Glassmorphism léger
- Animations fluides

## 🗺️ Architecture de l'Application

### Flux d'authentification

```
Splash Screen (3.5s)
       ↓
Login (Email/Téléphone/Biométrique)
       ↓
Sélection du profil
       ↓
Dashboard (rôle spécifique)
```

### Rôles et Dashboards

#### 1. **Femme Enceinte** 👩
**Route:** `/dashboard/pregnant`

Tableau de bord mobile-first avec:
- Suivi de la semaine de grossesse
- Constantes vitales (FC, SpO₂, Température, Tension)
- Mouvements du bébé
- Prochain rendez-vous
- Médicaments et traitement
- Conseils quotidiens (nutrition, hydratation, exercice)
- Navigation par onglets: Accueil, Historique, IA, Consultations, Profil
- Bouton SOS d'urgence flottant

#### 2. **Sage-femme** 👨‍⚕️
**Route:** `/dashboard/midwife`

Gestion des patientes avec:
- Vue d'ensemble des statistiques (patientes, grossesses à risque, consultations)
- Liste des patientes avec statut de santé
- Planning des rendez-vous
- Alertes urgentes
- Activité récente
- Gestion des demandes de téléconsultation

#### 3. **Gynécologue** 👩‍⚕️
**Route:** `/dashboard/gynecologist`

Diagnostic avancé avec:
- Cas médicaux complexes
- Imagerie médicale (échographies)
- Résultats d'examens
- Comparaison historique
- Facteurs de risque et prédictions IA
- Rapports exportables (PDF)
- Prescriptions électroniques

#### 4. **Agent Communautaire** 📍
**Route:** `/dashboard/community` (Placeholder)

Suivi en zone rurale:
- Femmes suivies
- Planification des visites
- Cartographie GPS
- Mode hors ligne avec synchronisation
- Scanner QR Code
- Gestion des urgences

#### 5. **Parent/Conjoint** 👥
**Route:** `/dashboard/family` (Placeholder)

Application simplifiée:
- Suivi de la grossesse
- Notifications
- Position GPS
- Calendrier des rendez-vous
- Accès SOS

## 🔧 Pages et Fonctionnalités

### Pages implémentées

1. **Splash Screen** (`/`)
   - Animation de démarrage
   - Logo BAYA
   - Tagline
   - Redirection automatique vers login

2. **Login** (`/login`)
   - Authentification par email, téléphone, ou biométrie
   - Sélecteur de langue (FR, EN, FON, YO, BAR)
   - Mode sombre
   - Mot de passe oublié
   - Création de compte

3. **Sélection du Profil** (`/profile-selection`)
   - 5 cartes de rôles avec couleurs spécifiques
   - Descriptions et icônes
   - Navigation vers les dashboards correspondants

4. **Dashboard Femme Enceinte** (`/dashboard/pregnant`)
   - Suivi santé complet
   - Gestion des vitals
   - Navigation mobile
   - SOS d'urgence

5. **Dashboard Sage-femme** (`/dashboard/midwife`)
   - Gestion de patientes
   - Statistiques et alertes
   - Planning

6. **Dashboard Gynécologue** (`/dashboard/gynecologist`)
   - Cas médicaux avancés
   - Gestion du risque
   - Rapports

7. **Assistant IA BAYA** (`/ai-assistant`)
   - Chat médical 24/7
   - Suggestions rapides
   - Analyse de risque
   - Orientation vers professionnels

8. **404 Not Found** (`*`)
   - Page personnalisée avec navigation

### Pages en développement (Placeholders)

- `/biomedical-results` - Résultats de laboratoire
- `/teleconsultation` - Consultations vidéo
- `/alerts` - Système d'alertes
- `/map` - Cartographie des patientes
- `/notifications` - Centre de notifications
- `/settings` - Paramètres utilisateur

## 📱 Responsive Design

L'application est optimisée pour:
- **Desktop:** Layouts complets avec sidebars
- **Tablet:** Adaptation flexible des grilles
- **Mobile:** Navigation par onglets, layouts empilés

Breakpoints Tailwind utilisés:
- `sm` (640px)
- `md` (768px)
- `lg` (1024px)
- `xl` (1280px)
- `2xl` (1536px)

## 🚀 Technologies

### Frontend
- **React 18** - Interfaces utilisateur
- **React Router 6 (SPA)** - Routage
- **TypeScript** - Type safety
- **Tailwind CSS 3** - Styling
- **Vite** - Build tool
- **Lucide React** - Icons
- **Framer Motion** - Animations
- **Radix UI** - Composants accessibles

### Backend
- **Express** - API server
- **Node.js** - Runtime

### State Management
- **React Query** - Gestion des données asynchrones
- **React Hooks** - État local

## 🎯 Fonctionnalités Clés

### Design System Complet ✅
- Palettes de couleurs
- Typographie
- Composants réutilisables
- États (hover, disabled, loading)
- Animations et transitions

### Authentification ✅
- Multiple auth methods (email, phone, biometric)
- Sélection de langue
- Mode sombre
- Profils utilisateurs

### Suivi de Santé ✅
- Constantes vitales
- Mouvements du bébé
- Médicaments
- Conseils personnalisés

### Intelligence Artificielle ✅
- Chat médical IA
- Suggestions rapides
- Analyse de risque
- Orientation automatique

### Gestion de Patientes ✅
- Listes avec filtrage
- Alertes prioritaires
- Statuts de santé
- Historique

### Navigation & UX ✅
- Bottom tabs (mobile)
- Responsive grids
- Smooth transitions
- Glass effect cards

## 📦 Structure des Fichiers

```
client/
├── pages/
│   ├── Splash.tsx                 # Écran de démarrage
│   ├── Login.tsx                  # Connexion
│   ├── ProfileSelection.tsx        # Sélection du rôle
│   ├── DashboardPregnant.tsx      # Dashboard femme enceinte
│   ├── DashboardMidwife.tsx       # Dashboard sage-femme
│   ├── DashboardGynecologist.tsx  # Dashboard gynécologue
│   ├── AIAssistant.tsx            # Chat IA BAYA
│   ├── Placeholder.tsx            # Pages en développement
│   └── NotFound.tsx               # Page 404
├── components/
│   └── ui/                        # Composants Radix UI
├── global.css                     # Thème et styles globaux
└── App.tsx                        # Routeur principal

tailwind.config.ts                 # Configuration Tailwind
```

## 🎨 Customization Guide

### Modifier les couleurs
1. Éditez `client/global.css` - Variables CSS HSL
2. Mettez à jour `tailwind.config.ts` si nécessaire
3. Les couleurs BAYA sont définies dans les custom colors

### Ajouter une nouvelle page
1. Créez `client/pages/MonPage.tsx`
2. Importez-la dans `App.tsx`
3. Ajoutez la route `<Route path="/mon-page" element={<MonPage />} />`

### Modifier le thème
- **Couleurs:** `client/global.css` (variables CSS)
- **Typographie:** `tailwind.config.ts` (fontFamily)
- **Rayon des coins:** `borderRadius` config
- **Animations:** Keyframes personnalisées

## 🔐 Sécurité

- Pas de données sensibles en frontend
- Validation Zod pour les entrées
- CORS configuré
- Routes protégées (à implémenter)

## 🚀 Prochaines Étapes

### À faire (Phase 2)
1. **Authentification Backend**
   - Implémentez JWT
   - Sécurisez les routes
   - Gestion des sessions

2. **Base de Données**
   - Schéma utilisateurs
   - Historique médical
   - Constantes vitales

3. **Features Avancées**
   - Intégration IA réelle
   - Imagerie médicale
   - Notifications push
   - Mode hors ligne

4. **Pages Restantes**
   - Dashboard communautaire
   - Dashboard famille
   - Résultats biomédicaux
   - Système de cartographie

5. **Tests & QA**
   - Tests unitaires (Vitest)
   - Tests d'intégration
   - Tests E2E

## 📊 Metrics & Analytics

À implémenter:
- Nombre de patientes suivies
- Taux de compliance
- Alertes traitées
- Temps moyen de consultation
- Taux de satisfaction

## 📞 Support

Pour améliorer ou ajouter des fonctionnalités:
- Mentionnez la fonctionnalité souhaitée
- Décrivez le contexte d'usage
- Précisez le rôle utilisateur concerné

### Exemples:
- "Ajoute une page de résultats biologiques avec graphiques de tendance"
- "Crée un système de notifications push pour les alertes urgentes"
- "Implémente le mode hors ligne avec synchronisation"

---

**BAYA v1.0** - Plateforme de Santé Numérique  
*Parce que chaque battement compte.*
