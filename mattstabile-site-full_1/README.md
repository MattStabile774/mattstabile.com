# MattStabile.com — New Static Site

A fast, free-to-host replacement for the Squarespace site, restyled in a modern editorial look (inspired by persumedia.com) and optimized for the search term **"Quant Finance Recruiter NYC / New York City."**

## What's included

```
index.html        Home (hero, specialties, FAQ, JSON-LD structured data)
about.html        About Matt
speaking.html     Speaking engagements (replaces old /video page)
contact.html      Contact info + form
blog/index.html   Blog index (placeholder, ready for posts)
css/styles.css    All styling
sitemap.xml       For Google Search Console
robots.txt        Allows crawling, points to sitemap
vercel.json       Clean URLs + 301 redirects from old Squarespace paths
```

## Deploy for free (recommended: Vercel)

1. Create a free account at vercel.com (sign in with GitHub is easiest).
2. Push this folder to a GitHub repo (or drag-and-drop the folder at vercel.com/new).
3. Vercel deploys it instantly — no build step needed.
4. In Vercel → Project → Settings → Domains, add `mattstabile.com` and `www.mattstabile.com`.
5. At your domain registrar, follow Vercel's DNS instructions (an A record to 76.76.21.21 and a CNAME for www).
6. Once DNS propagates, cancel Squarespace hosting.

Cloudflare Pages and Netlify work identically if you prefer them — all three are free for a site this size.

## ⚠️ Before canceling Squarespace: download your images

The pages currently hot-link images from Squarespace's CDN so you can preview immediately. **Those URLs will die when your Squarespace subscription ends.** Before canceling:

1. Download each image (headshot, the two lifestyle photos, logo) from the current site.
2. Save them into an `/images/` folder here with these names (or update the HTML):
   - `images/matt-stabile-headshot.jpg`
   - `images/matt-stabile-recruiting.jpg`
   - `images/matt-stabile-speaking.jpg`
   - `images/matt-stabile-founder.jpg`
3. Find-and-replace the `images.squarespace-cdn.com` URLs in the HTML files with the local paths.

Tip: keep the descriptive, keyword-rich alt text — it helps SEO.

## Contact form setup (free)

The form on `contact.html` uses Formspree (free tier: 50 submissions/month):
1. Sign up at formspree.io and create a form pointed at Matt@Stabilesearch.com.
2. Copy your form ID and replace `YOUR_FORM_ID` in `contact.html`.

Alternative: delete the form and rely on the mailto/phone links already on the page.

## SEO checklist after launch

Already built in:
- Title tags and H1s targeting "Quant Finance Recruiter NYC / New York City"
- Meta descriptions, canonical URLs, Open Graph tags
- JSON-LD structured data: Person, ProfessionalService (areaServed: New York City), and FAQPage
- Keyword-rich FAQ section, image alt text, internal linking
- sitemap.xml + robots.txt
- 301 redirects from old Squarespace URLs (/about-matt, /video, /home) to preserve existing link equity

To do after launch:
1. Add the site to Google Search Console (verify via DNS in Vercel) and submit sitemap.xml.
2. Do the same in Bing Webmaster Tools.
3. Update your LinkedIn profile and Stabile Search site to link to mattstabile.com — backlinks from relevant profiles matter.
4. Set up a free Google Business Profile ("Recruiter" category, New York, NY) — this is the single biggest lever for "quant finance recruiter NYC" local searches.
5. Publish blog posts targeting long-tail terms ("quant researcher salary NYC," "how to get a job at a quant fund," "hiring ML researchers in finance"). One post a month compounds quickly.
6. Cross-link between mattstabile.com and stabilesearch.com.

## Old Squarespace blog posts

If you have blog posts on the current site you want to keep, each becomes a folder: `/blog/post-slug/index.html`. Copy the card pattern in `blog/index.html` for the listing. Happy to migrate them — just share the URLs.
