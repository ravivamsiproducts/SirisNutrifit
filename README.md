# SirisNutriFit

Responsive nutrition and diet-consultation website prototype.

## Current website

- Main page: `My-Store/index.html`
- Root entry point: `index.html` redirects visitors to the main page for GitHub Pages.
- Responsive navigation for mobile and desktop.
- Service sections for weight management, personalized diet plans, consultation options, and progress tracking.
- Accessibility improvements: skip-to-content link, visible keyboard focus, reduced-motion support, and a back-to-top control.

## Important implementation status

The current site is a **front-end prototype**. Customer sign-in, registration, consultant/admin dashboards, diet-plan storage, appointment booking, payment processing, and notifications are not connected yet. Do not treat the Customer Login or consultation links as a working booking/authentication system until the backend integration is implemented and tested.

## Planned build sequence

1. Set up a dedicated SirisNutriFit Supabase project/schema (do not reuse unrelated store databases).
2. Implement secure customer authentication and profile ownership.
3. Add consultant-assigned diet plans and customer progress tracking with Row Level Security.
4. Add appointment requests and consultant/admin management.
5. Integrate payments and notification workflows only after the server-side security rules are in place.
6. Test mobile, accessibility, and account permissions before publishing to the production branch.

## Preview and publishing

This work is being prepared on the `nutrition-homepage` branch. Review it before merging into `main`. If GitHub Pages is configured for `main` and the repository root, the new root `index.html` forwards visitors to `My-Store/`.

## Safety

Never commit Supabase service-role keys, payment-gateway secret keys, passwords, or other server secrets into this repository. Only public client keys may be used in browser code, with Row Level Security and server-side validation correctly configured.
