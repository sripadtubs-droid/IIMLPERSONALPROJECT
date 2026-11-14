# Taskflow — Task Manager

A lightweight task manager built with React + Vite. It includes task creation/editing, completion tracking, a monthly calendar, due-date status, and a progress dashboard.

## Features

- Create, edit, delete, and complete tasks
- Due dates, priority, category, and optional notes
- Dashboard counts for due today, overdue, pending, and completed tasks
- Monthly calendar with task markers; select a day to see its tasks
- Search and filter tasks
- Data persists in the browser using `localStorage`
- Responsive layout for desktop and mobile

## Run locally

Requires Node.js 18 or newer.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite (usually http://localhost:5173).

## Build

```bash
npm run build
npm run preview
```

## Publish to GitHub

1. Create a new empty repository on GitHub.
2. Unzip this project.
3. In a terminal, open the unzipped folder and run:

```bash
git init
git add .
git commit -m "Add Taskflow task manager"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

## Deploy to Vercel

1. Sign in to Vercel and choose **Add New → Project**.
2. Import your GitHub repository.
3. Vercel should detect Vite automatically.
4. Keep the defaults:
   - Build command: `npm run build`
   - Output directory: `dist`
5. Select **Deploy**.

The included `vercel.json` supports client-side routing if you add routes later.

## Data and privacy

Tasks are stored in the current browser's `localStorage`. This means:
- No account or backend is required.
- Data stays in that browser on that device.
- Clearing browser storage or using another browser/device will not carry tasks over.

For cross-device sync, accounts, or shared task lists, connect a database such as Supabase in a future version.
