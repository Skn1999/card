# Contact card: NFC + QR

Live URL (once pushed): **https://skn1999.github.io/card/**

| File | What it is |
|---|---|
| `index.html` | The contact page: photo, email, phone, LinkedIn, portfolio, "Save to contacts" |
| `sumit-nayyar.vcf` | Contact file (vCard 3.0, photo included); the page's save button downloads it |
| `photo.jpg` | Page photo |
| `qr/qr-contact.png` / `.svg` | QR → `https://skn1999.github.io/card/?s=qr` |
| `print/lockscreen-s22plus-1080x2340.png` | S22+ lock-screen wallpaper with the QR |
| `print/business-cards-A4.pdf` | 10 cards (85 × 55 mm) on A4, one-sided, cut along the dashed lines |

The `?s=qr` / `?s=nfc` part makes the portfolio link carry `utm_medium=qr` or `utm_medium=nfc`, so your analytics show which one recruiters used.

## 1. Publish on GitHub Pages (5 min)

1. Create a new **public** repo on GitHub named `card` (no README).
2. In this folder, run:
   ```bash
   git init -b main
   git add index.html sumit-nayyar.vcf photo.jpg qr README.md NFC-SETUP.md
   git commit -m "Contact card"
   git remote add origin https://github.com/skn1999/card.git
   git push -u origin main
   ```
3. Go to the repo → **Settings → Pages** → Source: *Deploy from a branch*, Branch: `main` / `(root)` → Save.
4. Wait 1–2 minutes, then open https://skn1999.github.io/card/ on your phone and tap **Save to contacts**.

The `print/` folder stays local. Leave it out of the commit.

## 2. Before tomorrow

- [ ] The page loads on your phone
- [ ] Scan the wallpaper QR with a second phone (or a friend's iPhone) and save the contact
- [ ] Set `print/lockscreen-s22plus-1080x2340.png` as your lock screen: Gallery → ⋮ → Set as wallpaper → Lock screen
- [ ] Print `business-cards-A4.pdf` at **100% / Actual size** (not "Fit to page"), on thick paper if you have it
- [ ] Optional: NFC, see `NFC-SETUP.md`
