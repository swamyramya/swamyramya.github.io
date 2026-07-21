# SwaRam wedding site

Three self-contained pages (no build step, no dependencies):

| File         | Who it's for            | URL after publishing                          |
|--------------|-------------------------|-----------------------------------------------|
| `index.html` | Everyone (neutral)      | `https://USERNAME.github.io/REPO/`            |
| `groom.html` | Groom-side guests       | `https://USERNAME.github.io/REPO/groom.html`  |
| `bride.html` | Bride-side guests       | `https://USERNAME.github.io/REPO/bride.html`  |

## Publish on GitHub Pages (no command line needed)
1. Create a **new public repository** (e.g. `swaram-wedding`).
2. On the repo page click **Add file -> Upload files**, drag in `index.html`, `bride.html`, `groom.html` (and this README), then **Commit changes**.
3. Go to **Settings -> Pages** (left sidebar, under "Code and automation").
4. Under **Build and deployment -> Source**, pick **Deploy from a branch**.
5. Set **Branch** to `main`, folder `/ (root)`, then **Save**.
6. Wait ~1-3 min, refresh the Pages screen, and your live URL appears at the top.

Tip: for the cleanest possible address `https://USERNAME.github.io/` (no repo name),
name the repository exactly `USERNAME.github.io`.

## Before you share the links
The RSVP form runs in preview mode until you paste your Google Apps Script URL.
In each of the 3 files find `RSVP_ENDPOINT` and `GUESTLIST_URL` near the top of
the <script> block and paste your deployed Web App URL + Sheet URL. Re-upload to update.
