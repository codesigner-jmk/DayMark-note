# Daymark

Daymark is a local-first task and notes workspace built with React, Vite, Tailwind CSS, Lucide, Motion, date-fns, React Hook Form, and Tiptap.

## Run locally

```sh
pnpm install
pnpm dev
```

The production build is `pnpm build`; Vercel can deploy this directory with its Vite preset. App data is stored in the browser under `daymark-data` in localStorage. There is no account or server-side storage.

## Included

- Today, upcoming, overdue, all tasks, completed, project, tag, archive, and trash views
- Quick task creation and inline task details, priorities, status, tags, due/start dates, estimates, reminders, recurrence, and subtasks
- Recurring task completion schedules the next occurrence
- Local task notes and standalone rich-text notes with autosave
- Search across tasks, notes, projects, and tags (`⌘/Ctrl + K`)
- Overview with useful workload and weekly completion summaries
- Focus timer, light/dark/system appearance, responsive mobile navigation, and undoable task deletion

## Data shape

The local store keeps `tasks`, `projects`, `tags`, `notes`, and `settings` as separate collections. Each task and note has its own stable ID. This structure is intentionally simple to inspect and migrate without a backend.
