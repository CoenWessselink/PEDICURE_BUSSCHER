# Joanne Busscher Pedicure Borne — premium website

Live-ready statische website voor Joanne Busscher Pedicure Borne.

## Contactgegevens
- Telefoon: 06-54331250
- E-mail: joannebusscher@live.nl
- Adres: Veldovenweg 17, 7621 GR Borne
- Afspraaksoftware: SARA SalonSoft

## Lokaal draaien
```powershell
npm install
npm run dev
```

## Build
```powershell
npm install
npm run build
```

## Cloudflare Pages
- Build command: `npm run build`
- Output directory: `dist`

Let op: `https://pedicure-busscher.pages.dev/` toont meestal de production branch van Cloudflare, vaak `main`.
Als de wijzigingen alleen naar `feature/podofile-premium-website` zijn gepusht, ziet u ze niet op de production URL totdat de branch is gemerged naar `main` of Cloudflare op deze branch is ingesteld.

## Afspraaklink aanpassen
De knoppen gebruiken nu `BOOKING_URL` in `script.js`.
Vervang deze door de persoonlijke SARA SalonSoft boekingslink zodra deze beschikbaar is.
