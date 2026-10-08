# Brightdesk Commercial Cleaning (portfolio demo)

A one-page quote request page for an Australian after-hours commercial cleaning company. Visitors pick the kind of premises they need cleaned (office, clinic, venue, shop, school, strata, warehouse or other), add their contact details, and land on a thank-you screen with a mock site-visit calendar and a simulated AI-callback notice. Choosing "a private home" shows a polite "we only clean business premises" screen instead.

Live demo: https://historfic.github.io/brightdesk-commercial-cleaning/

## About this project

Brightdesk Commercial Cleaning is a fictional brand, and this page is a portfolio piece. It is not a real business.

- **No backend.** The site is a static export of a Next.js + Tailwind page: HTML, CSS and JavaScript only. The fonts are self-hosted, so the page loads nothing from other sites.
- **Nothing is collected or sent.** The form checks what you type, then discards it. No requests are made, nothing is stored, and no cookies are set. A Content-Security-Policy blocks network calls and form submission.
- **The booking calendar is a mock.** It shows sample times, and picking one books nothing.
- **The AI phone call is simulated.** No call is placed.
- **The phone numbers are fictional** and use the Australian ranges set aside for drama and examples. The email address uses example.com.
- The client sectors are generic labels, and the owner and the client reviews are invented.

## Run locally

The page is built to live at `/brightdesk-commercial-cleaning/`, so serve it from a parent folder:

```bash
mkdir -p ../preview
cp -r . ../preview/brightdesk-commercial-cleaning
cd ../preview && python -m http.server 8000
```

Then open http://localhost:8000/brightdesk-commercial-cleaning/.
