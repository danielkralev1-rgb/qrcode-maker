SiteStock QR — Firestore (GitHub Pages friendly)

What you get:
- Single HTML file that reads/writes to Firebase Firestore (multi-user, realtime).
- Anonymous auth (no sign-up screens).
- Still works as a static site — perfect for GitHub Pages.

Quick setup
1) Create a Firebase project: https://console.firebase.google.com
2) Firestore Database → Create database.
3) Project settings → "Add app" → Web → copy the config.
4) Open the HTML file, paste your config into the firebaseConfig block.
5) Firestore Rules → paste rules from Firebase_Firestore_Rules.txt → Publish.
6) Commit the HTML to a GitHub Pages repo (or deploy to Netlify/Cloudflare Pages).
7) Open the site; it will auto sign in anonymously and sync.

Collections
- items (doc id = SKU): sku, desc, site, bin, uom, min, max, onhand, deleted
- transactions (auto-id): ts (serverTimestamp), user, type, sku, qty, ref
