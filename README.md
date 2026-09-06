# ossig-reprochallenge

Static website for the OHBM-OSSIG Reproducibility Challenge, built with [Eleventy (11ty)](https://www.11ty.dev/), Nunjucks templates, plain CSS, and vanilla JavaScript.

## Local Deployment (Run Locally)

1. Install dependencies:

```bash
npm install
```

2. Start local development server:

```bash
npx @11ty/eleventy --serve
```

Open http://localhost:8080/ossig-reprochallenge/.

## Deployment

GitHub Actions workflow is defined in `.github/workflows/deploy.yml`:

- Trigger: push to `main`
- Build: `npx @11ty/eleventy`
- Deploy target: `gh-pages` branch

In the upstream repository's **Settings → Pages**, use **Deploy from a branch**
with the `gh-pages` branch and `/ (root)` folder. The Eleventy base path is
`/ossig-reprochallenge/`, matching the repository name.

## Repository

https://github.com/ohbm/ossig-reprochallenge

## Website

https://ohbm.github.io/ossig-reprochallenge/

## More Info

[OSSIG Website](https://ossig.netlify.app/challenge/)
