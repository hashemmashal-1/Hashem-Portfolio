# Hashem Mashal — Portfolio

A zero-cost, responsive personal portfolio with **Light / Dark mode**, individual project case-study pages, and room for future deliverables, images, documentation, and prototype embeds.

Built with React + Vite + custom CSS. Hosted on Cloudflare Pages (free plan).

## Run locally

1. Install Node.js 20+.
2. From this folder run `npm install`.
3. Run `npm run dev` for a local preview.
4. Run `npm run build` to produce the deployable `dist/` folder.

## Deployment (Cloudflare Pages)

1. Push this project's files to your GitHub `Hashem-Portfolio` repository (not the ZIP itself).
2. In Cloudflare: Workers & Pages → Create → Pages → Connect to Git.
3. Select `hashemmashal-1/Hashem-Portfolio`.
4. Framework preset: **Vite**; build command: `npm run build`; build output directory: `dist`.
5. Deploy. Cloudflare provides a free `*.pages.dev` address.

## Update project content

All project metadata and writeups are in `src/data.js`. Add/update entries inside the `projects` array. Project page URLs follow `#/projects/<slug>`.

- Put PDFs in `public/docs/` and add links to the corresponding project's `resources` array, e.g. `{label:'BRD (PDF)', url:'/docs/rashfa-brd.pdf'}`.
- Put images in `public/images/`; use image paths when expanding project sections.
- Link publicly shareable Figma prototypes in project `resources` after reviewing sharing permissions. An interactive iframe embed can be added to the case-study page later.
- Never publish employer/client proprietary documents, confidential data, private credentials, or unapproved project artifacts.

## Content disclosure

Project summaries are based on documented CV details and prior RASHFA planning. RASHFA is labeled *in progress*, TrackFlow a *self-initiated case study*, and Sanus a *graduation project*. Placeholder artwork is **not** a screenshot of a real product.

## Design

The theme button persists the preferred light/dark appearance in local storage; first visits follow the operating-system preference. Both themes work at desktop and mobile sizes.
