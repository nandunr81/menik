# Menik & Co. – Ad landing page

Static landing page for Menik & Co. (wholesale calibrated Ceylon gemstones), built for Google Ads and Reddit Ads traffic.

- `index.html` – the whole page (HTML, CSS and a small script, no build step)
- `assets/` – logo marks, gem cut-outs and photos

## Conversion tracking
The page pushes these events to `window.dataLayer`: `generate_lead` (quote form sent), `whatsapp_click`, `email_click`. Add your Google Ads / Reddit Pixel tags (or Google Tag Manager) in `<head>` to pick them up.

## Quote form
There is no form backend yet: on submit the visitor's email app opens with the request filled in, addressed to kasunrgems@gmail.com. Connect a form service (e.g. Formspree, Netlify Forms) to receive submissions directly.
