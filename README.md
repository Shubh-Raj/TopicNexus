# 🧠 Topic Nexus

**Topic Nexus** is a modern, full-stack discussion platform built using Next.js 15, Prisma, and Tailwind CSS. It supports authentication, rich UI interactions, and a clean developer experience — ideal for building community discussions or topic-based Q&A apps.

---

## 🚀 Features

- ✅ Full-stack app with Next.js App Router
- 🔐 User authentication (NextAuth.js with Prisma adapter)
- 🧵 Create and manage discussion snippets
- 🎨 Fully styled using Tailwind CSS and Radix UI
- ⚡ Powered by Turbopack (dev mode)
- 🧠 Form validation using Zod

---

## 📦 Tech Stack

### Frontend
- **Next.js 15.3.2** – App Router, SSR, Optimized Build
- **React 19** – UI Framework
- **Tailwind CSS 4** – Utility-first styling
- **Radix UI** – Accessible UI primitives (`avatar`, `dialog`, `popover`, etc.)
- **Lucide React** – Icon set

### Backend & Auth
- **Prisma 6** – ORM for database management
- **@auth/core** & **next-auth@5 (beta)** – Authentication
- **@auth/prisma-adapter** – Auth DB adapter for Prisma

### Validation
- **Zod** – Type-safe schema validation

---

## 🛠 Dev Setup

### 1. Install dependencies

```bash
npm install
````

### 2. Setup `.env` file

```env
DATABASE_URL=your_database_url
NEXTAUTH_SECRET=your_auth_secret
NEXTAUTH_URL=http://localhost:3000
```

### 3. Prisma setup

```bash
npx prisma init
npx prisma migrate dev --name init
npx prisma generate
```

### 4. Start dev server

```bash
npm run dev
```

---

## 🏗 Build for Production

```bash
npm run build
npm start
```

---

## 📁 Project Structure

```
/app           → App directory (App Router)
 /actions      → Server actions (e.g. createSnippet)
 /components   → Reusable UI components
 /lib          → Prisma client, utilities
 /styles       → Tailwind & globals
 /prisma       → schema.prisma + migrations
```

---

## 📚 Scripts

| Command         | Description                     |
| --------------- | ------------------------------- |
| `npm run dev`   | Start dev server with Turbopack |
| `npm run build` | Create production build         |
| `npm start`     | Start production server         |
| `npm run lint`  | Run ESLint                      |

---

## ✍️ Author

**Shubh** — built for portfolio/discussion-based app use case.

---
