# Heldspace website (for App Store & AdMob)

Minimal one-page site so you can verify Heldspace in AdMob and satisfy App Store links. **Free** via GitHub Pages, no domain needed.

---

## 1. Before you start

- Replace the App Store link in `index.html`: change `idXXXXXXXXX` to your real app ID (e.g. `id1234567890`).
- Optional: edit `privacy.html` with your real privacy policy text later.

---

## 2. Option A: Your own GitHub user site (recommended — shortest URL)

Your site will be **https://YOUR-USERNAME.github.io** and **https://YOUR-USERNAME.github.io/app-ads.txt**.

1. Create a GitHub account: https://github.com/join  
2. Create a **new repository**:
   - Name: **YOUR-USERNAME.github.io** (e.g. if your username is `johndoe`, use `johndoe.github.io`)
   - Public, no README
3. Upload the contents of this `website` folder to the **root** of that repo:
   - `app-ads.txt`
   - `index.html`
   - `privacy.html`
4. Turn on Pages: **Settings** → **Pages** → Source: **Deploy from branch** → Branch: **main** → **Save**.
5. After a minute or two, check:
   - https://YOUR-USERNAME.github.io
   - https://YOUR-USERNAME.github.io/app-ads.txt

---

## 3. Option B: Project repo (e.g. “heldspace”)

Your site will be **https://YOUR-USERNAME.github.io/heldspace** and **https://YOUR-USERNAME.github.io/heldspace/app-ads.txt**.

1. Create a new repo named e.g. **heldspace** (public, no README).
2. Upload the contents of this `website` folder to the **root** of that repo.
3. **Settings** → **Pages** → Source: **Deploy from branch** → Branch: **main** → **Save**.
4. Check:
   - https://YOUR-USERNAME.github.io/heldspace
   - https://YOUR-USERNAME.github.io/heldspace/app-ads.txt

---

## 4. App Store Connect

- **Privacy Policy URL**: set to your site’s base URL (e.g. `https://YOUR-USERNAME.github.io` or `https://YOUR-USERNAME.github.io/heldspace`) or to the privacy page (e.g. `https://YOUR-USERNAME.github.io/privacy.html`).
- **App Store** → Your app → **App Information** → paste that same URL in the field Apple uses for privacy/developer site.

---

## 5. AdMob

- In AdMob, for **Heldspace (iOS)**, set the app website / verification URL to the **exact same** base URL (e.g. `https://YOUR-USERNAME.github.io` or `https://YOUR-USERNAME.github.io/heldspace`).
- Run verification again. AdMob will fetch **https://YOUR-BASE-URL/app-ads.txt** and should succeed.

---

## 6. Summary

| Where              | URL to use |
|--------------------|------------|
| App Store (Privacy / Developer) | Your GitHub Pages base URL |
| AdMob (app website) | Same base URL |
| app-ads.txt        | That base URL + `/app-ads.txt` |

The domain AdMob checks is the host of the URL you give (e.g. `YOUR-USERNAME.github.io`). As long as `app-ads.txt` is at that host’s root (or in the path you set for the project site), verification will work.
