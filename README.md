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

## Site to-do

Waiting on content:

- [ ] Convocation photos for the Boston chapter of the story
- [ ] Google New York event photo (replaces the "photos coming soon" card)
- [ ] Résumé PDF updated to Portland, OR (phone number removed before upload)
- [ ] Medium article link for "How Transformers work"
- [ ] Side projects: year, one more line each, GitHub links
- [ ] Headline choice (current, or one of the journey-led options)

To check:

- [ ] GAN paper title: Google Scholar says "Conversation of real images into cartoonize image
      format", the site says "Conversion … cartoonized". Match the published PDF everywhere.
- [ ] Job title: site and résumé say "AI Engineer, Clinical Data"; match the offer letter.

Add as they happen:

- [ ] Each published article or paper in Research & writing
- [ ] Each completed peer review or judging role in Service
- [ ] Talks, press and events
