# shreyaasoba.com

Personal site. One static HTML file, no build step, no dependencies.

## Editing

Open `index.html` and edit it. That is the whole workflow. Push to `main` and Cloudflare
Pages redeploys automatically.

To preview locally, open the file in a browser, or serve it:

```bash
python3 -m http.server 8000
```

## Deployment

Hosted on Cloudflare Pages, connected to this repository. Every push to `main` deploys.

**Build settings in the Pages dashboard:**

| Setting | Value |
|---|---|
| Framework preset | None |
| Build command | *(leave empty)* |
| Build output directory | `/` |

## Things to keep in sync

The `<head>` contains a `schema.org` JSON-LD block listing ORCID, Google Scholar, LinkedIn
and GitHub under `sameAs`. That block is what tells search engines these profiles belong to
one person. If a profile URL changes, update it there too.

Cross-links currently in place:

- ORCID &rarr; Scholar, LinkedIn, GitHub
- This site &rarr; ORCID, Scholar, LinkedIn, GitHub

Still to add: the site URL on ORCID, Google Scholar, LinkedIn and the GitHub profile, so the
links point both ways.
