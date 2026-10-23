# School Personal LMS (y3t1-lms)

A personal study site for my Year 3, Term 1 Software Engineering courses at Western. It renders my Obsidian course notes and runs practice quizzes for each course. Built with Next.js, with Markdown, KaTeX math and Mermaid diagrams.

| Course | Topic |
|---|---|
| ECE 4436A | Networking |
| SE 3309A | Database Management Systems |
| SE 3310A | Theoretical Foundations of Software Engineering |
| SE 3316A | Web Technologies |
| SE 3351A | Software Project and Process Management |
| SE 3352A | Software Requirements and Analysis |

## Run it

The app is published as a Docker image:

```bash
docker run -d --name lms -p 3000:3000 ghcr.io/colebranston/school_personal_lms:latest
```

Then open http://localhost:3000.

## What's in this repo

| Path | Contents |
|---|---|
| `content/` | Course notes (synced from my Obsidian vault), one folder per course with `Content/` (definitions) and `Note/` (lecture notes) |
| `quizzes/` | Practice quiz banks, one JSON file per course |
| `public/vault-images/` | Images referenced by the notes |
| `server.js`, `package.json` | Production server entry point and dependencies |

> **Note:** this repo was recovered from the running container, which only holds the compiled Next.js build. The original app source (pages/components, `next.config.mjs`, and the `scripts/sync-notes.mjs` / `scripts/check-quizzes.mjs` helpers) isn't included, so `npm run build` won't work from here. Use the Docker image above to run the app.
