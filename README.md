# PUST Cover Page Generator

A browser-based PDF cover page generator for PUST (Pabna University of Science and Technology) students. Fill in your course and student details, preview a live A4 cover, and export a pixel-perfect PDF — entirely in the browser, no server required.

## Tech Stack

- **React 19** — UI framework
- **Vite** — build tool and dev server
- **html2canvas + jsPDF** — client-side PDF generation

## Local Development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
# Output: dist/
```

## Deploy to Vercel

### One-click import

1. Go to [vercel.com/new](https://vercel.com/new) and import the `shoruvx/pdf_generator` repository.
2. Vercel automatically detects **Vite** as the framework. The settings below are filled in automatically — verify they match:

   | Setting | Value |
   |---|---|
   | **Framework Preset** | Vite |
   | **Build Command** | `npm run build` |
   | **Output Directory** | `dist` |
   | **Install Command** | `npm install` |

3. No environment variables are required for this project.
4. Click **Deploy**.

### SPA routing

The included `vercel.json` rewrites all routes to `index.html` so client-side navigation works correctly after a hard refresh or direct URL visit.

### Subsequent deployments

Every push to `main` will trigger an automatic deployment on Vercel once the project is imported.
