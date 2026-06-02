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
De persoonlijke SARA SalonSoft link is ingesteld op `https://JoanneBusscherPedicure.sarasalonsoft.nl`.

## Logo
Het originele aangeleverde logo is opgenomen als `assets/logo-joanne-busscher-pedicure-borne.png` en wordt gebruikt in header, footer en CTA.

## SARA SalonSoft
- Boekingslink: https://JoanneBusscherPedicure.sarasalonsoft.nl
- Publiek te boeken dagen: dinsdag, woensdag en donderdag
- Klantnummer en gebruikersnaam zijn niet op de publieke website geplaatst.

## SARA iframe integratie
De SARA boekingsapp is geïntegreerd op de pagina in de sectie `#online-afspraak`.

Gebruikte iframe:
```html
<iframe name='boekingappframe' id='onlineBoeken' width='100%' scrolling='yes' style='overflow-x:hidden;overflow-y:auto;height:500px' src='https://JoanneBusscherPedicure.boekingapp.nl?cid=16569&CategoryId=197147'></iframe>
```

In de website is de hoogte verhoogd naar 760px voor betere weergave binnen de premium lay-out.

## Definitieve publieke boekingslink
De publieke SARA/BoekingApp-link is ingesteld op:
https://joannebusscherpedicure.boekingapp.nl

Cloudflare fix:
- package-lock.json is verwijderd zodat er geen interne sandbox registry meer wordt gebruikt.
- .npmrc forceert de publieke npm registry.
