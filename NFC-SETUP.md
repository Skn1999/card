# NFC setup

The tag stores only a link: **`https://skn1999.github.io/card/?s=nfc`**
iPhones (XS and newer) and Android phones open a link from a tag with no app needed, and the page does the rest.

## Option A: try your NFC button first (2 min)

1. Install **NFC Tools** (wakdev) on your S22+. It's free.
2. Turn NFC on: Settings → Connections → NFC and contactless payments.
3. NFC Tools → **Read**, then hold the button to the middle of the phone's back.
4. Look at **Writable**:
   - **Yes:** go to **Write → Add a record → URL/URI**, paste `https://skn1999.github.io/card/?s=nfc`, then **Write** and hold the button to the phone again. Read it once more to check.
   - **No / locked:** the button can't be reused. Use Option B.

Don't tap **"Lock tag"** in Other. It's permanent.

## Option B: buy NTAG215 stickers (for the next events)

- Search for "NTAG215 NFC sticker" or "NFC tag card". A pack costs a few euros at Verkkokauppa.com, Clas Ohlson or online.
- **NTAG213/215/216** all work. Avoid "MIFARE Classic", because iPhones can't read it.
- Stick it on the back of your phone case. If the case has a **metal** plate or MagSafe ring, use an "anti-metal" tag instead.
- Write it the same way as in Option A.

## How to use it with a recruiter

"Tap your phone here." They hold the top of their iPhone (or the middle of an Android's back) to your tag, and a link notification pops up. If nothing happens within 2 seconds, show the QR on your lock screen instead.

Their phone needs to be unlocked. On Android, NFC must also be on, and it's sometimes off.

## Why not phone-to-phone?

- Apple's NameDrop only works between iPhones and isn't open to other apps.
- Samsung Wireless PowerShare is charging only; it carries no data.
- Your S22+ *can* pretend to be a tag (Host Card Emulation), but that needs an extra app and is unreliable with iPhones. A €2 sticker does the same job better.
