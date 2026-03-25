# Helsesjekk – STERK Helse & Trening

Digitalt spørreskjema for pasienter som skal til helsesjekk.

## 🔒 Personvern

- **Ingen data sendes til noen server** – alt behandles lokalt i pasientens nettleser
- **Ingen cookies, analytics eller sporing**
- PDF-en genereres lokalt via jsPDF og lagres kun på pasientens enhet
- Pasienten sender selv PDF-en via [Pasientsky](https://www.pasientsky.no)

## 🌐 URL

Skjemaet er tilgjengelig på: **https://helsesjekk.sterkmedisinske.no**

## 📋 Slik fungerer det

1. Pasienten mottar en lenke til skjemaet per e-post
2. Fyller ut skjemaet i nettleseren (fungerer på iPhone, iPad, Android og PC/Mac)
3. Laster ned PDF lokalt på sin enhet
4. Logger inn på Pasientsky og sender PDF-en som vedlegg til klinikken

## 🛠 Teknisk

- Én enkelt HTML-fil (`index.html`) – ingen backend, ingen database
- Hostet via GitHub Pages med custom domain
- jsPDF lastes fra CDN for PDF-generering
- Google Fonts (Lora + DM Sans) for typografi
- iOS-kompatibel PDF-nedlasting (blob-URL med del-dialog)

## 📁 Filstruktur

```
├── index.html   ← Selve skjemaet
├── CNAME        ← Custom domain for GitHub Pages
└── README.md    ← Denne filen
```

## ⚙️ Oppsett

1. Opprett et nytt repo på GitHub
2. Last opp alle filene i dette repoet
3. Gå til Settings → Pages → velg «Deploy from a branch» → `main`
4. Under Custom domain, skriv `helsesjekk.sterkmedisinske.no` og aktiver «Enforce HTTPS»
5. Hos domeneregistraren: legg til CNAME-record: `helsesjekk` → `BRUKERNAVN.github.io`

DNS-endringer kan ta opptil noen timer.
