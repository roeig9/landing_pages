# landing_pages

Roei Grimberg's static landing pages, served by Netlify.

- `/` — generic page for small businesses (`index.html`)
- `/boostapp` — page for Boostapp marketplace customers (`boostapp/index.html`)
- `/scan` — free Google Maps presence check form; posts to the n8n workflow at `rgconsultant.app.n8n.cloud/webhook/business-scan` (`scan/index.html`)
- `/report-assets/` — page template (`template.txt`) and edit panel (`admin.txt`) for scan reports. The n8n report viewer downloads them on each view, so changing them changes how every report looks. Generated from the n8n project; not linked from the site.
- `/book` — redirect to the booking calendar that logs the click source in Google Analytics (`book/index.html`). Link as `/book?from=report&biz=<business name>`.

No build step. Netlify publish directory: repository root.
