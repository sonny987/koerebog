# Kørebog Pro 🚗

Erhvervskørsel webapp til firmaer med QR-scanning, GPS og automatisk km-tæller OCR.

## Funktioner

- **QR-scanning**: Scan bil-koden → starter erhvervskørsel automatisk
- **Km-tæller OCR**: Tag billede af km-tæller → aflæses automatisk med AI
- **GPS-tracking**: Beregner distance præcist undervejs
- **Auto privat-registrering**: Kørsel over 15 km/t uden scanning = privat
- **Spørg-funktion**: Spørger om erhverv/privat ved ukendt kørsel
- **Månedlig rapport**: Oversigt, diagram, kørselsgodtgørelse
- **CSV export**: Til bogføring/SKAT
- **PWA**: Installer som app på telefonen

## Hurtig hosting via GitHub Pages (gratis)

1. Opret konto på github.com
2. Opret nyt repository (fx "koerebog")
3. Upload de 3 filer: index.html, sw.js, manifest.json
4. Gå til Settings → Pages → Deploy from branch: main
5. Din app er tilgængelig på: https://[dit-navn].github.io/koerebog

## Eller Netlify (drag & drop)

1. Gå til netlify.com → Log in
2. Træk mappen ind på "Deploy manually"
3. Færdig! Du får en URL med det samme.

## QR-kode setup i bilen

1. Åbn appen → Indstillinger
2. Skriv bilens nummerplade
3. Tryk "Generer QR-kode"
4. Print og sæt i bilen (rude, instrumentbræt)

## SKAT kørselsgodtgørelse 2025
- Sats: 3,79 kr/km (standard, justerbar i indstillinger)
- Rapporten beregner automatisk godtgørelse pr. måned

## Teknologi
- Rent HTML/CSS/JS — ingen server nødvendig
- Tesseract.js til OCR (klient-side AI)
- Html5-QRCode til scanning
- localStorage til data
- GPS via browser Geolocation API
- PWA til offline + installation
