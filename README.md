# Longreen Lawn Care — Quotes & Invoices

A self-contained pricing and invoicing app for Longreen Lawn Care.

## Publish it on GitHub Pages

1. Create a new GitHub repository (public repos get free Pages hosting).
2. Upload **all the files in this zip** — `index.html`, `manifest.json`,
   `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` — to the root of
   that repository (drag-and-drop on github.com, or `git add` / `commit` /
   `push` if you're using git locally).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to **Deploy from a branch**,
   pick the `main` branch and the `/ (root)` folder, then **Save**.
5. GitHub will give you a URL like `https://<your-username>.github.io/<repo-name>/`
   — that's your live app. It usually takes a minute or two to go live after
   the first push.

## Add it to your phone's home screen

Once the site is live at your github.io URL, open that link in your phone's
browser, then:

**iPhone (Safari):**
1. Tap the **Share** icon (square with an arrow) in the toolbar.
2. Scroll down and tap **Add to Home Screen**.
3. Tap **Add** in the top right.

**Android (Chrome):**
1. Tap the **⋮** menu in the top right.
2. Tap **Add to Home screen** (or **Install app**, if it shows up).
3. Confirm by tapping **Add** / **Install**.

Either way, you'll get a Longreen icon on your home screen that opens the
app full-screen, without the browser's address bar — it behaves like a
regular installed app from there.

## A couple of things to know

- The app saves your settings, customers, and job history in the browser's
  local storage. That means data is tied to whichever browser/device you're
  using it on — it won't automatically sync between your phone and laptop,
  and clearing your browser data (or uninstalling/reinstalling the home
  screen icon) will clear it too.
- PDF downloads on the invoice screen use a small library loaded from a CDN,
  so an internet connection is needed for that button to work.
- All the pricing logic lives in the `DEFAULT_CONFIG` object near the top of
  the `<script>` tag in `index.html`, and is also editable live from the
  in-app Settings page — no code changes needed for day-to-day price updates.
