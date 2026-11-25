# Menik Co – Ad landing page

Static landing page for Menik Co (menikco.com) (wholesale calibrated Ceylon gemstones), built for Google Ads and Reddit Ads traffic.

- `index.html` – the landing page (HTML, CSS and a small script, no build step)
- `standard-calibrated-sizes.html` – full size chart
- `matching-sets.html` – standard matching sets ("See all sets")
- `custom-sets.html` – customised set-making process ("View more"; process copy is marked as draft)
- Links to `index.html?req=<type>#quote` preselect the request type in the quote form
- `assets/` – logo marks, gem cut-outs and photos
- Smooth scrolling by [Lenis](https://github.com/darkroomengineering/lenis) 1.3.27 (loaded from unpkg); menu links stop below the sticky menu, and it switches off for visitors who prefer reduced motion

## Conversion tracking
The page pushes these events to `window.dataLayer`: `generate_lead` (quote form sent), `whatsapp_click`, `email_click`. Add your Google Ads / Reddit Pixel tags (or Google Tag Manager) in `<head>` to pick them up.

## Quote form
There is no form backend yet: on submit the visitor's email app opens with the request filled in, addressed to kasunrgems@gmail.com. Connect a form service (e.g. Formspree, Netlify Forms) to receive submissions directly.

## Placeholders to replace
- `assets/hero-gem-mine.jpg` – stand-in photo from a web search; replace with Menik Co's own gem-mine photo before running ads.
- Packaging photos still show the old "Menik & Co." name.
