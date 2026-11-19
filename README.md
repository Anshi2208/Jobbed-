# Jobbed 🎀

### A private, pretty place to keep track of the jobs you’ve applied for.

Jobbed helps you organize applications and keep the details you’ll want to look back on—all in one place. Add your resume, note whether you used a cover letter, view the full application details, and keep track of each application’s progress.

> **Your search, your records.** Jobbed is an application tracker, not a job-search board.

## ✨ Features

- **Home dashboard** — application totals and a status chart for applied, interview, offer, rejected, and withdrawn applications.
- **Applications table** — search and filter your records, view or edit details, and remove applications. Row colors distinguish statuses: green for applied, blue for interview, purple for offer, and red for rejected or withdrawn.
- **Application details** — review the job title, company, description, date, status, notes, and posting link.
- **Resume and cover letter tracking** — privately attach the resume you used; record whether you used a cover letter, with an optional attachment.
- **Recruiter message drafts** — generate an editable message using your saved resume, optional cover letter, and job description, then copy it to review and send yourself.
- **Personal profile** — add your name, major, and profile photo. Preview, drag, and zoom to crop a photo before saving; the avatar gets a little bow, too. 🎀
- **Private accounts** — sign in with email and password. Supabase row-level security and storage policies keep each account’s records and uploads separated.

## 🔐 Privacy notes

- Application and profile rows use Supabase row-level security, scoped to the signed-in user.
- Resumes, cover letters, and profile photos are stored in private buckets. Photo links are signed and temporary.
- Resume and cover-letter files can be PDF, DOC, or DOCX up to 10 MB. Profile photos can be JPG, PNG, or WebP up to 5 MB.
- Recruiter drafts are generated only when you choose **Generate draft**. Jobbed extracts text on the local server and sends it with the job description to Groq. The Groq API key stays on the server, and drafts are not sent to recruiters automatically.

## 🗂️ Project layout

```text
database/                 Supabase schema and row/storage policies
public/                   Browser UI, styles, and MVC-style JavaScript
  css/
  js/controllers/
  js/models/
  js/views/
server/                   Local Node.js server and API configuration
  services/               Recruiter draft generation
package.json              Document text-extraction dependencies
start-jobbed.bat          Windows launcher
```

## 🛠️ Built with

- Vanilla JavaScript, HTML, and CSS
- Node.js
- Supabase Auth, Postgres, and private Storage
- Groq API and PDF, DOC, and DOCX text extraction

## 📸 Screenshots

> Personal names, photos, and application details have been obscured in these public previews.

- **Sign In Page**
  
  <img width="323" height="337" alt="image" src="https://github.com/user-attachments/assets/360d0488-1b50-4767-b33d-45ae25b73ec5" />

<br>

- **Home dashboard**
  
<img width="943" height="469" alt="image" src="https://github.com/user-attachments/assets/6953faa8-2aa5-4c45-9b8e-3b945ba27800" />

<br>

- **Applications dashboard**
  
<img width="945" height="196" alt="image" src="https://github.com/user-attachments/assets/e4653f3c-70f6-474e-9b0a-c568c1e3ef12" />

<br>

- **Personal profile**
  
<img width="592" height="372" alt="image" src="https://github.com/user-attachments/assets/ae6c3138-6c09-4da1-97f4-1c4748a4f427" />

- **Application details — Recruiter Message Draft**
<img width="746" height="160" alt="image" src="https://github.com/user-attachments/assets/053146bb-19fc-4e80-b971-758e2ad3f2ce" />

