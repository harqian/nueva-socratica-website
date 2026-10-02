# nueva-socratica-website

static site for nuevasocratica.com. `public/` is what gets served.

- push to main -> `.github/workflows/deploy.yml` -> `wrangler pages deploy public` -> cloudflare pages project `nueva-socratica-website` (account b5767c459ae1102e08c8dd559b76ee15). secret `CLOUDFLARE_API_TOKEN` = the pages-only token.
- dns: cloudflare zone nuevasocratica.com (registrar hostinger, NS charles/grannbo.ns.cloudflare.com). apex + www are proxied CNAMEs -> nueva-socratica-website.pages.dev.
- planned: lunchline.nuevasocratica.com for ~/code/lunch_line_monitor.
