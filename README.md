# ExecutiveFlow AI

AI-powered executive assistance: email organisation, task extraction, calendar assistance, executive briefings and administrative automation.

**ExecutiveFlow AI is a [YomieVerse](https://yomie-commits.github.io/Yomie-Verse/) product.**

Live site: https://yomie-commits.github.io/ExecutiveFlowAI/

Sister products: [SocialFlow AI](https://yomie-commits.github.io/SocialFlowAI/) · [ExecutiveFlow AI](https://yomie-commits.github.io/ExecutiveFlowAI/) · [LeadFlow AI](https://yomie-commits.github.io/LeadFlowAI/)

## Structure

| Path | What it is |
|---|---|
| `index.html` | Product page: hero, features, how it works, demo, pricing, FAQ, enquiry form |
| `privacy.html`, `thank-you.html`, `404.html` | Supporting pages |
| `build.py` | Generates every page, the sitemap, robots.txt and the favicon. Page copy is in the `P` dictionary and `build_index()` near the bottom |
| `assets/css/site.css` | YomieVerse design system v3, themed in teal |
| `assets/js/config.js` | **Settings you can change without rebuilding**: email, WhatsApp, booking link, analytics |
| `assets/js/main.js` | Menu, animations and the enquiry form (shared with YomieVerse) |
| `assets/img/` | Favicon and social share image |

After editing `build.py`, run `python3 build.py` and commit the regenerated HTML.

## Notes

- **Enquiry form:** delivered by [FormSubmit](https://formsubmit.co) to the email in `config.js`. The first real submission triggers a one-time "Activate Form" email; click its link once.
- **Live demo:** the Demo section links to the AI Executive Assistant demo workspace at https://yomie-commits.github.io/automationservices/app/ (it lives in the automationservices repository).
- **Hosting:** GitHub Pages, `main` branch, root folder.
- **Theme colour substitutions** applied to the YomieVerse stylesheet: #7c5cff→#0d9488, #6a48f0→#0f8a7f, #5534d6→#0f766e, #efebff→#ddf5f1, #b6a6ff→#7ee8d6, #c4b5ff→#99f0e0, #8fb0ff→#7dd3fc, rgb 124,92,255→13,148,136, rgb 85,52,214→15,118,110, `--violet`→`--brand`.
- **Placeholders:** the privacy notice needs a "last updated" date.
