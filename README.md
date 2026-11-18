# Jobbed 🎀

### A private, pretty place to keep track of the jobs you’ve applied for.

Jobbed helps you organize applications and keep the details you’ll want to look back on—all in one place. Add your resume, note whether you used a cover letter, and keep track of each application’s progress.

> **Your search, your records.** Jobbed is an application tracker, not a job-search board.

## ✨ Features

- **Home dashboard** — application totals, awaiting responses, interviews, offers, and other outcomes.
- **Applications table** — search and filter your records, then edit or remove them.
- **Application details** — save the job title, company, description, date, status, notes, and posting link.
- **Resume and cover letter tracking** — privately attach the resume you used; record whether you used a cover letter, with an optional attachment.
- **Personal profile** — add your name, major, and profile photo. Preview, drag, and zoom to crop a photo before saving; the avatar gets a little bow, too. 🎀
- **Private accounts** — sign in with email and password. Supabase row-level security and storage policies keep each account’s records and uploads separated.

## 🔐 Privacy notes

- Application and profile rows use Supabase row-level security, scoped to the signed-in user.
- Resumes, cover letters, and profile photos are stored in private buckets. Photo links are signed and temporary.
- Resume and cover-letter files can be PDF, DOC, or DOCX up to 10 MB. Profile photos can be JPG, PNG, or WebP up to 5 MB.

## 🗂️ Project layout

```text
database/                 Supabase schema and row/storage policies
public/                   Browser UI, styles, and MVC-style JavaScript
  css/
  js/controllers/
  js/models/
  js/views/
server/                   Local Node.js server and API configuration
start-jobbed.bat          Windows launcher
```

## 🛠️ Built with

- Vanilla JavaScript, HTML, and CSS
- Node.js
- Supabase Auth, Postgres, and private Storage

## 📸 Screenshots

> Personal names, photos, and application details have been obscured in these public previews.

- **Sign In Page**
  
  <img width="673" height="687" alt="Sign In Page" src="https://github.com/user-attachments/assets/ab879a10-7bb5-45ad-9564-81cf0ed417ec" />

<br>

- **Home dashboard**
  
  <img width="1555" height="768" alt="Home dashboard" src="https://github.com/user-attachments/assets/a3986248-d6ea-48e7-81ec-c9ee491a7f7b" />

<br>

- **Applications dashboard**
  
  <img width="1559" height="768" alt="Applications dashboard" src="https://github.com/user-attachments/assets/a0f154d1-8e73-4cc1-b709-7ce6500093b0" />

<br>

- **Personal profile**
  
  <img width="1201" height="751" alt="Personal profile" src="https://github.com/user-attachments/assets/5c16e75a-7ca2-4a0a-a75a-c52eda5c463f" />

