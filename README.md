# landing_pages

Roei Grimberg's static landing pages, served by Netlify.

- `/` — generic page for small businesses (`index.html`)
- `/boostapp` — removed; redirects to `/?utm_source=boostapp` (`_redirects`)
- `/scan` — free Google Maps presence check form; posts to the n8n workflow at `rgconsultant.app.n8n.cloud/webhook/business-scan` (`scan/index.html`)
- `/report-assets/` — page template (`template.txt`) and edit panel (`admin.txt`) for scan reports. The n8n report viewer downloads them on each view, so changing them changes how every report looks. Generated from the n8n project; not linked from the site.
- `/intake` — intake questionnaire for a new client (not linked, noindex): services, prices, FAQ, what the bot hands off, tone. Saves a draft in the browser; posts to the n8n workflow at `rgconsultant.app.n8n.cloud/webhook/business-intake`, which emails Roei the answers and a draft bot knowledge file (`intake/index.html`)
- `/book` — redirect to the booking calendar that logs the click source in Google Analytics (`book/index.html`). Link as `/book?from=report&biz=<business name>`.

No build step. Netlify publish directory: repository root.
