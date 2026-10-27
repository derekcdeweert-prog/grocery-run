# Grocery Run

Gedeelde boodschappenlijst als losse webapp (GitHub Pages + Firebase).

## 1. Firebase (eenmalig, ~10 min)
1. Ga naar console.firebase.google.com, log in met Google, **Add project** → naam `grocery-run` (Analytics mag uit).
2. **Build → Authentication → Get started** → zet **Google** en **Email/Password** aan.
3. **Authentication → Settings → Authorized domains** → voeg `derekcdeweert-prog.github.io` toe.
4. **Build → Firestore Database → Create database** → locatie `eur3 (europe-west)` → production mode.
5. Firestore → tab **Rules** → vervang alles door de inhoud van `firestore.rules` → **Publish**.
6. Projectinstellingen (tandwiel) → **Your apps** → web-icoon `</>` → naam `grocery-run` → kopieer het `firebaseConfig`-blok naar `config.js`.

## 2. GitHub Pages
1. Nieuwe repository `grocery-run` op github.com, upload alle bestanden.
2. **Settings → Pages** → Source: *Deploy from a branch*, branch `main`, map `/ (root)`.
3. Na een minuut staat de app op `https://derekcdeweert-prog.github.io/grocery-run/`.

## 3. Op de iPhone
Open de link in Safari → deelknop → **Zet op beginscherm**. Log in, tik op het poppetje rechtsboven en voeg het e-mailadres van je partner toe. Zij doet hetzelfde op haar telefoon en ziet dezelfde lijst.

Zonder `config.js` ingevuld draait de app in demomodus (niets wordt bewaard of gedeeld).
