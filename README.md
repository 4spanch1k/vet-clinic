# VetCare Clinic — business card website

Lab work No. 9 (ICT6001): a responsive, mobile-first website for a veterinary clinic.

## Components

| # | Component | What it does |
|---|-----------|--------------|
| 1 | Header / Nav | Flex/grid bar; burger menu on phones (checkbox + label, no JS); "Call Doctor 24/7" button |
| 2 | Hero | Medical illustration (WebP with SVG fallback), H1 "Professional Care for Your Pets", CTA "Make an Appointment" |
| 3 | Grid sections | Services (Therapy, Surgery, Vaccination) and Staff: 1 column on mobile, 12-column grid on desktop |
| 4 | Feedback form | Pet's Name, Pet Species, Owner's Phone, Email, date picker; `required`, `type="tel"`, `type="email"`, validation states in pure CSS |
| 5 | Footer | Emergency phone, address, messengers, legal block, night-mode (theme inversion) switch |

## Tech notes

- Semantic HTML5 only: `header`, `nav`, `main`, `section`, `article`, `footer` (no `div`).
- CSS Grid + Flexbox; relative units (`rem`, `%`, `vh`, `vw`); the only pixel value is the required `@media (min-width: 1024px)` breakpoint.
- Light / dark themes via `color-scheme` + `light-dark()`; text contrast checked against WCAG AA.
- Mobile-first: primary actions live in a bottom dock (thumb zone) on phones.
- Squircle corners via `corner-shape: squircle` where supported, with rounded fallback.

## Structure

```
index.html
style.css
images/    SVG icons and illustrations, hero.webp
```

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Contact details, address and staff names are placeholders for demonstration.
