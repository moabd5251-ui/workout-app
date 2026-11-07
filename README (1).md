# Workout Log — Trainer App

A complete training tracker: gym + no-gym programs, Pilates, cardio, multi-person
profiles, progress charts, and dose tracking. Installs on any phone as an app.

---

## Setup — step by step (about 5 minutes)

### 1. Sign in to github.com (create a free account if needed)

### 2. Create the repository
- Tap the **+ (plus) icon** in the top-right corner → **New repository**
- **Repository name:** `workout-app`
- Select **Public** (required for the free app link)
- Leave everything else as-is — don't check any boxes
- Tap the green **Create repository** button

### 3. Upload the app files
- The next page shows a wall of code instructions — ignore it
- Find the line near the top: *"…or **uploading an existing file**"* — tap that link
- Unzip this zip file first, then select/drag in everything that was inside the
  `workout-app` folder:
  - `index.html`
  - `manifest.json`
  - `sw.js`
  - `icon-192.png` and `icon-512.png`
  - `README.md`
  - the **`.github` folder** (contains the auto-deploy workflow)
- Tap the green **Commit changes** button

> **If the `.github` folder won't upload (common on phones):** upload the other
> files first and commit. Then in the repo tap **Add file → Create new file**,
> type this exact name in the filename box:
> `.github/workflows/deploy.yml`
> (typing the slashes creates the folders), paste the contents of the
> `deploy.yml` file from this zip into the big text box, and tap **Commit changes**.

### 4. Turn on the app hosting
- In your repo, tap the **Settings** tab (top of the page)
- In the left menu tap **Pages**
- Under **Build and deployment → Source**, choose **GitHub Actions**

### 5. Done — open your app
Wait about 1 minute (the **Actions** tab shows the deploy running, green check = live).
Your app address is:

```
https://YOUR-USERNAME.github.io/workout-app/
```

Replace `YOUR-USERNAME` with your actual GitHub username.

---

## Installing it on a phone
Open the app link in the phone's browser:
- **Android (Chrome):** menu (⋮) → **Add to Home screen** → Install
- **iPhone (Safari):** Share button → **Add to Home Screen**

It opens full-screen like a native app and works offline after the first visit.

## Sharing with clients
Just text them the link. Each phone keeps its own private data — nobody sees
anyone else's logs. The in-app **Back up data / Restore** buttons move data
between devices if ever needed.

## Updating the app later
Open `index.html` in the repo → tap the **pencil icon** → replace the contents
with the new version → **Commit changes**. The GitHub Action redeploys
automatically; phones get the new version on their next online visit.
