# Placement Management System

## 🎓 Overview

A full-stack Placement Management System for colleges to simplify and digitize the campus placement process.

## 🛠️ Tech Stack

| Layer          | Technology                     |
|----------------|--------------------------------|
| Frontend       | React.js, Vite, Tailwind CSS   |
| Backend        | Node.js, Express.js            |
| Database       | MySQL                          |
| ORM            | Prisma (Code First)            |
| Authentication | JWT, bcrypt                    |
| File Upload    | Multer                         |

## 📁 Project Structure

```
placement-management-system/
├── backend/
│   ├── prisma/
│   │   └── schema.prisma         # Database models
│   ├── src/
│   │   ├── controllers/          # Request handlers
│   │   ├── routes/               # API route definitions
│   │   ├── middleware/            # Auth & upload middleware
│   │   ├── utils/                # Helper functions
│   │   ├── generated/            # Prisma generated client
│   │   ├── prismaClient.js       # Prisma singleton
│   │   └── server.js             # Express entry point
│   ├── uploads/                  # Uploaded files (resumes)
│   ├── .env                      # Environment variables
│   ├── .env.example              # Env template
│   └── package.json
│
├── frontend/
│   └── src/
│       ├── components/           # Reusable UI components
│       ├── pages/                # Page components
│       ├── services/             # API service layer (Axios)
│       ├── context/              # React context (Auth, etc.)
│       └── App.jsx               # Root component
│
├── docs/                         # Project guidelines & documentation
│   ├── UI_DESIGN_SYSTEM.md       # Complete UI visual guide & exact Tailwind classes
│   ├── DEVELOPMENT_WORKFLOW.md   # Beginner handbook: 4 steps to build & submit PRs
│   ├── ISSUES_BACKLOG.md         # 12 pre-scoped issues ready to open in GitHub
│   ├── BACKEND_API_CONTRACT.md   # Live backend endpoints & response shapes
│   ├── FRONTEND_GUIDELINES.md    # Frontend styling & Tailwind standards
│   └── ROADMAP.md                # Milestones & feature matrix
│
├── .gitignore
└── README.md
```

## 📚 Club Guidelines & Documentation

For all Software Developers Club (SDC) contributors:
* 🎨 **[Unified UI Design System](docs/UI_DESIGN_SYSTEM.md):** **Must Read for UI!** Exact Tailwind classes for Buttons, Cards, Colors, Badges, and Tables.
* 🚀 **[Contributor Handbook](docs/DEVELOPMENT_WORKFLOW.md):** The 4 simple steps to pick a task and send a PR.
* 📋 **[Frontend Issues Backlog](docs/ISSUES_BACKLOG.md):** 12 ready-to-copy GitHub issues for your sprint.
* 🔌 **[Backend API Contract](docs/BACKEND_API_CONTRACT.md):** Real backend endpoints you can connect to today.
* 🗺️ **[Product Roadmap](docs/ROADMAP.md):** Milestone breakdown across Student, TPO, and Admin tracks.




## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)
- MySQL Server
- Git

### Backend Setup

```bash
cd backend
npm install
```

Update the `.env` file with your MySQL credentials:

```env
DATABASE_URL="mysql://root:yourpassword@localhost:3306/placement_db"
JWT_SECRET="your-super-secret-jwt-key"
```

Run Prisma migrations:

```bash
npx prisma migrate dev --name init
npx prisma generate
```

Start the server:

```bash
npm run dev
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

## 👥 User Roles

| Role     | Description                                      |
|----------|--------------------------------------------------|
| Admin    | Manage users, TPO accounts, monitor system       |
| TPO      | Manage students, companies, drives, eligibility  |
| Student  | View drives, update profile, upload resume       |

## 📊 Database Models

- User
- Student
- StudentSkill
- Company
- PlacementDrive
- EligibilityCriteria
- EligibleBranch
- PlacementStatus
- Notification
- Resume

## 📜 License

This project is licensed under the MIT License.
