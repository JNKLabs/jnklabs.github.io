# jnklabs.github.io

The JNK Labs website (games & apps): home page, privacy policy, contact form and `app-ads.txt` (for AdMob).

## Before uploading, replace these
1. Contact email: `jnklabssupport@gmail.com` (in `index.html` JSON-LD, the contact form's FormSubmit `action`, and `privacy.html`).
   The contact form uses FormSubmit (free): send yourself one test message after publishing and click the confirmation link it emails you.
2. `app-ads.txt` already has the AdMob publisher ID (pub-8661978230190789); check it matches AdMob → Apps → app-ads.txt
   (AdMob → Apps → View all apps → app-ads.txt → copy the line AdMob shows).
3. In `privacy.html`, check the **Luttapi & Ghosts** and **SYNC** sections match what those apps really do,
   then delete the `<!-- ... -->` notes.
4. When Ring Unlock is live, change its "Coming soon" button in `index.html` to its Play Store link.

## Publish (free, GitHub Pages)
1. Create a GitHub account with the username **jnklabs**.
2. Create a public repository named **jnklabs.github.io**.
3. Upload every file in this folder (keep the `img` folder).
4. After a minute the site is live at https://jnklabs.github.io
   - privacy policy: https://jnklabs.github.io/privacy.html
   - app-ads.txt: https://jnklabs.github.io/app-ads.txt

## SEO after publishing
- Add the site to Google Search Console (https://search.google.com/search-console), verify it, and submit `https://jnklabs.github.io/sitemap.xml`.
- Test the structured data: https://search.google.com/test/rich-results
- If you move to a custom domain, replace `https://jnklabs.github.io` everywhere (canonical, og:url, JSON-LD, sitemap.xml, robots.txt, form `_next`).

## Then, in Google Play Console (for every app)
- Store presence → Store settings → **Website**: `https://jnklabs.github.io`
- App content → **Privacy policy**: `https://jnklabs.github.io/privacy.html`

AdMob checks app-ads.txt within about 24 hours of the website being set in Play.

## Later: your own domain (e.g. jnklabs.in)
1. Buy the domain.
2. GitHub repo → Settings → Pages → **Custom domain**: enter `jnklabs.in` → Save (GitHub adds a `CNAME` file).
3. At the domain seller's DNS settings add:
   - four **A** records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - a **CNAME** record for `www` → `jnklabs.github.io`
4. Back in Settings → Pages, tick **Enforce HTTPS** once it's available (can take up to a day).
5. Update Play Console for every app: Website → `https://jnklabs.in`, Privacy policy → `https://jnklabs.in/privacy.html`.
   (The old jnklabs.github.io address keeps working: it redirects to the new domain.)
