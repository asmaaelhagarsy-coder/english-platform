
# English Platform – 1st Secondary (First Term)

This repository hosts a **single-file** interactive platform (HTML) with tabs for Units 1–6, British TTS, matching games, and an **English-only exam UI**.

## Files
- `index_unified_platform_v3.html` – main platform (open it directly or deploy on GitHub Pages).
- `assets/json/unit{1..6}_words.json` – per-unit word lists shown under the Unit Exam section.
- `assets/audio/correct.mp3` – optional success sound (fallback beep exists if not provided).

## Deploy on GitHub Pages
1. Create a **public** repo and upload all files.
2. Go to **Settings → Pages** → set **Branch: main** and **Folder: /root**.
3. Wait a minute; your site will be live at `https://<username>.github.io/<repo-name>`.

## Add Your Exam
Send your **Word (.docx)** for each unit. We'll convert it to **JSON** and plug it into the Exam UI so questions appear automatically (MCQ, T/F, gaps, matching).

## Add Matching Data
Edit `matchingData` inside the HTML and add pairs like:
```js
matchingData['u3-matching'] = [
  { term: 'deceive', meaning: 'يخدع' },
  { term: 'verify',  meaning: 'يتحقق' }
];
```

## Enable Sound
Click **Enable Sound** once (browser policy). We prefer a **slow British female voice** when available.
