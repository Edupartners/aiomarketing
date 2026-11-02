# aiomarketing.cz

Statický web (GitHub Pages, doména v `CNAME`). Bez build kroku: `index.html` + `assets/site.css`.

- `llms.txt`: přehled pro AI asistenty. Při změně ceníku nebo nabídky upravit spolu s `index.html` (text i JSON-LD).
- `assets/ukazka-mesicniho-reportu.pdf`: ukázka reportu vygenerovaná skriptem z repa `ortocentrum-ov/reporting` (ilustrativní data, označená jako ukázka).
- Měření: stránka volá `gtag('event', …)` pro `phone_click`, `email_click`, `report_download`, `faq_open`, `form_submit`, ale jen když je na stránce vložený Google Analytics. GA4 zatím vložený není; po vložení je potřeba doplnit i cookie lištu.
- Formulář nemá backend (GitHub Pages neumí PHP), otevírá e-mail s vyplněnou poptávkou. Později lze napojit na n8n webhook.
- Písma Plus Jakarta Sans (stejné jako v reportu) a IBM Plex Mono jsou hostovaná lokálně v `assets/fonts` (licence SIL OFL 1.1, z balíčků Fontsource).
