# Budgee

Application web de gestion de budget personnel avec utilisateurs, comptes, transactions, catégories, statistiques, et traductions.


Développé par Antoine RICHARD

## Fonctionnalités principales backend

- Authentification sécurisée (JWT, bcrypt)
- Gestion des utilisateurs (CRUD + reset mot de passe)
- Gestion des comptes bancaires (type, budget de départ)
- Gestion des transactions (ajout, édition, suppression)
- Gestion des catégories (globales par défaut + personnalisées)
- Duplication automatique des catégories par défaut à l'inscription
- Architecture RESTful claire (user, account, category, transaction)

## Fonctionnalités principales front-end

- Thème clair/sombre
- Internationalisation (français / anglais)
- Responsive design (mobile / desktop)
- Statistiques mensuelles (graphiques)
- Affichage des transactions récentes (tableau + cartes responsive)
- Page de profil (modification des infos, avatar, suppression)
- Formulaires sécurisés pour inscription, connexion, mise à jour

---

## Stack technique

### Backend

- **Node.js + Express**
- **MongoDB + Mongoose**
- **jsonwebtoken** (authentification)
- **bcrypt** (hash mot de passe)
- **CORS**

### Frontend

- **Vite + React**
- **Axios**
- **Chart.js**
- **i18next** (traduction)

---

### Structure du projet
```bash
/budgee
├── back/           # Backend Express (API REST)
├── front/          # Frontend React (Vite)
└── README.md       # Documentation
```

## Installation

### Prérequis

- [Node.js ≥ 18](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/try/download/community) (local ou [MongoDB Atlas](https://www.mongodb.com/cloud/atlas))

### Cloner le projet

```bash
git clone https://github.com/anto95240/Budgee.git
cd Budgee
```

### Backend
```bash
cd backend
npm install
```

Créer un fichier .env :
```bash
PORT=5000
MONGO_URI=mongodb://localhost:27017/project-db
JWT_SECRET=votre_secret_jwt
```

Démarrer le backend :
```bash
npm run dev
```

### Frontend
```bash
cd ../frontend
npm install
```

Créer un fichier .env.local :
```bash
VITE_API_URL=http://localhost:5000
```

Démarrer le frontend :
```bash
npm run dev
```

## Bonus

- Responsive design (mobile / desktop)

## Lien externe

Figma : https://www.figma.com/design/iHhUT56KhHDlVPIMZrzq64/DEV-WEB?node-id=28-311&t=YV4AYmS3wX8gDGhK-1

# Auteur
Développé avec par Antoine RICHARD
