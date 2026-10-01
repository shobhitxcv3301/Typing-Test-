# TypeFlow AI

Deployment-ready static build of the TypeFlow AI typing application.

## Included
- Typing practice: words, quotes, code, numbers and adaptive mode
- WPM, accuracy, errors, consistency and flow metrics
- Goals, streaks, history and local heatmap
- Local AI Coach
- Certification exam UI and printable certificate
- Local certificate lookup
- Theme/accent controls
- Local admin exam configuration
- Demo Pro subscription/checkout UI

## Deploy on Vercel
1. Put this folder in a Git repository.
2. Import the repository into Vercel.
3. Framework preset: **Other** / static site.
4. Build command: **leave empty**.
5. Output directory: **`.`**.
6. Deploy.

## Deploy on Netlify
Drag this folder into Netlify Drop, or connect the Git repository. No build command is required.

## Important production limitations
This build is a static frontend. User data, certificates and admin settings are stored in browser `localStorage`.

Therefore:
- Certificates cannot currently be verified across different devices/users.
- The admin password is present in client-side JavaScript and is not a secure server credential.
- The Pro checkout is a demonstration only; it does not charge cards or create a real subscription.
- Do not collect real card details with this demo checkout.

For a real public SaaS, the next production phase should add a backend/database, authenticated admin access, server-side certificate records/verification, and a real payment provider such as Stripe or Razorpay using tokenized checkout rather than handling card data in the frontend.
