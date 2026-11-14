# Personal Branding Website

A responsive executive-style portfolio built with Next.js, React, TypeScript and Tailwind CSS. It is prepared for GitHub and Vercel deployment.

## 1. Personalise the content

Most of the website content is centralised in `data/profile.ts`. Update:
- Name, initials, role, headline and introduction
- Email and LinkedIn URL
- About section
- Career history and achievements
- Expertise areas, projects and certifications

Replace every placeholder with accurate information. Do not publish confidential client, employer or project information.

### Profile image
The starter uses a typographic monogram in the hero section. To use a photograph, add an optimised image to `public/` and update the hero section in `app/page.tsx`.

### Resume
Add your PDF to `public/resume.pdf`. The download button is already configured to use this path. If you do not add a PDF, remove or temporarily hide the download button.

## 2. Run locally

Install Node.js 18.17 or newer.

```bash
npm install
npm run dev
```

Open http://localhost:3000.

To verify a production build:

```bash
npm run build
npm start
```

## 3. Publish to GitHub

1. Create a new empty repository on GitHub.
2. Extract this ZIP file.
3. Open a terminal in the extracted project folder.
4. Run:

```bash
git init
git add .
git commit -m "Initial personal branding website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

Replace the repository URL with your own GitHub repository URL.

## 4. Deploy on Vercel

1. Sign in at https://vercel.com using your GitHub account.
2. Select **Add New → Project**.
3. Import the repository you just created.
4. Keep the detected framework as **Next.js**.
5. No environment variables are required for the starter version.
6. Select **Deploy**.

Vercel will build and publish the website. Future pushes to the connected GitHub branch will trigger deployments automatically.

## 5. Contact form behaviour

The contact form validates the fields and opens the visitor's default email application using a pre-filled email. It does not store or transmit form submissions to a server. For a fully hosted form, connect a form service or implement a secure server-side endpoint.

## 6. Before going live

- Replace all placeholder content.
- Check every LinkedIn and email link.
- Add your real resume PDF.
- Review the site on mobile and desktop.
- Add a real profile photo if desired.
- Check that all public content is approved for sharing.
- Update the page title and description in `app/layout.tsx`.

## Project structure

```text
personal-branding-website/
├── app/
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components/
│   ├── ContactForm.tsx
│   └── Navigation.tsx
├── data/
│   └── profile.ts
├── public/
│   └── README-resume.txt
├── .gitignore
├── next.config.mjs
├── package.json
├── postcss.config.mjs
├── tailwind.config.ts
└── tsconfig.json
```
