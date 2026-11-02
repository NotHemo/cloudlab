# CloudLab — IT8417 Advanced Cloud Databases

[Open CloudLab](https://nothemo.github.io/cloudlab/)

Interactive Weeks 1–6: 41 lessons, six guided labs, 95 quiz questions, flashcards, revision, notes, and database practice. Built with Next.js, TypeScript, Tailwind CSS and browser-local PostgreSQL (PGlite). MongoDB and Redis exercises are explicitly simulated. Dark mode is the default. No paid APIs or database credentials are required.

## Source layout

The complete application was uploaded through the signed-in browser as three ZIP bundles to preserve all directory paths and stay within per-file upload limits. Download or clone this repository, then extract **all three** cloudlab-source-*.zip files into the same folder. They contain app/, components/, content/, lib/, public/, scripts/, tests/ and the package configuration. The archives include the source materials served by the learning platform.

The Pages workflow unpacks these bundles in its build workspace, runs the tests, exports the website with /cloudlab as its base path, and deploys out/. It has read-only source access and never pushes changes to this repository. If conventional unpacked source is added later, the workflow uses it directly.

## Run locally

Use Node.js 22 or newer. After extracting all bundles:

```sh
npm ci
npm test
npm run build
npm start
```

Open http://127.0.0.1:3000/. For development, use npm run dev. Leave NEXT_PUBLIC_BASE_PATH unset locally; Pages sets it to /cloudlab during deployment.

## Saved progress

Progress, bookmarks, notes and theme preferences are stored in your browser. The live site has separate storage from localhost. Use the notebook backup export/import controls to transfer progress.

The platform is for exam preparation. Follow your university rules, including the prohibition on AI during the exam.
