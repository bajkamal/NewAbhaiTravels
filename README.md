# New Abhai Travels

A single-page car, tempo traveller and bus rental website. Static HTML/CSS/JS — no build step, no backend. Booking is handled entirely through direct contact (call, WhatsApp, email), not an online payment flow.

## Structure

```
index.html                     Main site (hero, fleet, steps to book, about, testimonials, feedback, contact)
privacy-policy.html            Privacy Policy
terms-and-conditions.html      Terms & Conditions
cancellation-refund-policy.html  Cancellation & Refund Policy

herofinal.png                  Hero background photo
qr-code.png                    QR code used in the Feedback section

Crysta/, DZIRE/, Ertiga/,      Vehicle photo sets. Within each folder, the lowest-numbered
Fortuner/, WagonR/, XUV300/,   image is the fleet-card thumbnail; the rest populate the
tempo17/, tempo21/, tempo26/   modal gallery for that vehicle.

docs/                          Reference documents (not linked from the site)
archive/                       Old drafts and superseded reference files, gitignored
```

## Tech

- [Tailwind CSS](https://tailwindcss.com/) via CDN (no build step)
- [Phosphor Icons](https://phosphoricons.com/)
- Google Fonts: Syne (display) + Inter (body)
- Vanilla JavaScript — no framework

## Local development

No build step is required. Serve the folder with any static file server, e.g.:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/index.html`.

## Editing contact details

Phone, WhatsApp, and email are hardcoded in a handful of places in `index.html` (nav, hero, mobile bar, book section, vehicle modal). Search for `+919876543210` and `hello@newabhaitravels.com` to update them everywhere.
