# SkyNest — Soar High. Nest Well.

Complete travel website for flights & hotels with direct airline links, ready to launch.

## Full Project Structure

```
skynest/
├── index.html                 ← Homepage
├── manifest.json              ← PWA manifest
├── sw.js                      ← Service worker (offline-ready)
├── sitemap.xml                ← SEO sitemap
├── robots.txt
├── images/
│   ├── logo.svg
│   └── logo-icon.svg
├── pages/
│   ├── about.html
│   ├── contact.html
│   ├── privacy.html
│   ├── terms.html
│   ├── faq.html
│   ├── blog.html
│   ├── blog-cheapest-flights.html
│   └── destination-bali.html
├── emails/
│   ├── welcome.html
│   └── price-alert.html
├── social/
│   └── SOCIAL-KIT.md
├── docs/
│   └── API-INTEGRATION-PLAN.md
└── README.md
```

## What’s Included (All Next Steps Completed)

✅ Professional logo (SVG)  
✅ Extra pages: About, Contact, Privacy, Terms, FAQ, Blog, Destination guide  
✅ Full SEO: meta tags, Open Graph, Twitter cards, sitemap.xml, robots.txt  
✅ PWA support (installable on mobile, basic offline caching)  
✅ Real booking API integration plan (Duffel / Amadeus)  
✅ Email templates (Welcome + Price Alert)  
✅ Social media kit (bios, posts, hashtags, content pillars)  

## Quick Start

```bash
cd skynest
python3 -m http.server 8080
```
Open http://localhost:8080

## Launch Checklist

1. **Deploy** → Cloudflare Pages (recommended) or Netlify / Vercel  
2. **Domain** → skynest.travel (or skynesthq.com / getskynest.com)  
3. **Email** → hello@skynest.travel (Cloudflare Email Routing or ImprovMX)  
4. **Analytics** → Plausible or Google Analytics  
5. **Search Console** → Submit sitemap.xml  
6. **Socials** → Use the kit in `/social`  

## Brand

- **Name**: SkyNest  
- **Tagline**: Soar High. Nest Well.  
- **Colors**: Sky blue `#0ea5e9` / Navy `#0c4a6e` / Amber `#f59e0b`  
- **Logo**: `/images/logo-icon.svg` and `/images/logo.svg`

## Future Roadmap

See `/docs/API-INTEGRATION-PLAN.md` for moving from redirect model to live results and full booking.

---

**SkyNest is complete and ready for takeoff.**  
Deploy the folder, register the domain, and start welcoming travelers.
