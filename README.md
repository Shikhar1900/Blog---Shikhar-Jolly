# Idea Atlas — website starter

An editorial, responsive blog prototype with searchable/filterable article cards, article pages, reading time, auto-generated table of contents, and a Pages CMS content configuration. The publication name is provisional until the domain/brand is confirmed.

## Local preview
Run `python -m http.server 8000` from this directory and open `http://localhost:8000`. Running from a local server is important because the homepage fetches `content/articles.json`.

## Free hosting plan
- Public site: Cloudflare Pages Free, connected to a GitHub repository. Cloudflare Pages supports custom domains and automatic deployments from Git.
- Content editing: Pages CMS (`https://pagescms.org/`) connected to your GitHub repository. The `.pages.yml` file defines editable article and site-setting fields. Log in using your own GitHub account and grant access only to this repository.
- Domain: purchase a `.com` separately; registration is not free. Configure the domain in Cloudflare Pages and follow its DNS/nameserver instructions.

## Publish checklist
1. Create/sign in to GitHub and create a **private or public** repository. Pages CMS needs access; the public website's source can be public, but do not store secrets in it.
2. Upload the project files and commit them to the repository.
3. In Cloudflare, create a Pages project using **Connect to Git** and select the repository. For plain HTML, use no build command and set the output directory to `/` (or follow the current Cloudflare dashboard guidance).
4. Open Pages CMS, sign in with GitHub, select the repository, and confirm it reads `.pages.yml`. Use the Articles collection to edit the sample entries.
5. Add the custom domain from the Cloudflare Pages project settings and follow the DNS instructions.
6. Before launch, replace sample article drafts, verify the author bio, add favicon/social images, test mobile layouts, and review SEO metadata.

## Important notes
- This bundle is **not yet hosted publicly**. Hosting requires connecting your own GitHub and Cloudflare accounts and domain, which I cannot do without account authorization.
- Pages CMS is an external publishing dashboard; the site does not embed an admin password/login of its own. Repository access controls who can edit content.
- The sample article content is starter/demo text; replace it with your final writing before public launch.
- Free tiers and limits can change. Confirm terms before launch.
