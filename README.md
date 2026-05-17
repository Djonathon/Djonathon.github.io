# dmitrispiro.com

Personal portfolio site built with Jekyll, hosted on GitHub Pages.

## Setup

1. Create a GitHub repo named `Djonathon.github.io`
2. Push all files in this folder to that repo
3. Go to repo Settings → Pages → set source to `main` branch
4. Under Settings → Pages → Custom domain, enter `dmitrispiro.com`
5. At your domain registrar (wherever you bought dmitrispiro.com), add these DNS records:

**A records** (point @ to GitHub):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME record**:
```
www → Djonathon.github.io
```

## Swapping in the Beehiiv embed

In `index.html`, find the comment `<!-- Replace the form below with your Beehiiv embed code -->` and replace the `<div class="subscribe-form">...</div>` block with your Beehiiv script embed.

## Updating writing links

In `index.html`, update the `href` values on the `.writing-item` links to point to your actual article URLs.

## Adding your photo

Replace `assets/img/profile.jpeg` with any updated headshot. Keep the same filename or update the reference in `index.html`.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000
