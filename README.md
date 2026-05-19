# Tommaso Parrucchiere — Sito web

Sito vetrina moderno per **Tommaso Parrucchiere**, barbiere e parrucchiere uomo a Palermo.
Statico (HTML5 + CSS + JavaScript), mobile-first, ottimizzato per le prestazioni e la SEO locale.

## Struttura

```
tommaso-barbiere/
├─ index.html          Pagina unica (hero, studio, servizi, gallery, recensioni, prenota, mappa, footer)
├─ css/style.css       Design system dark / urban luxury
├─ js/main.js          Menu, scroll reveal, lightbox gallery
├─ images/             Foto e favicon
└─ README.md
```

## Come pubblicarlo

È un sito statico: basta caricare l'intera cartella su un qualsiasi hosting
(Netlify, Vercel, GitHub Pages, Aruba, ecc.) oppure aprire `index.html` nel browser.

Anteprima locale:

```bash
# dentro la cartella del progetto
python -m http.server 8000
# poi apri http://localhost:8000
```

## Cosa personalizzare prima della messa online

| Elemento | Dove | Note |
|---|---|---|
| **URL Facebook** | `index.html` (cerca `facebook.com/search`) — JSON-LD, footer | Sostituisci con il link reale della pagina Facebook |
| **Dominio** | `index.html` — tag `canonical`, `og:url`, `og:image` | Inserisci il dominio definitivo (ora: `tommasoparrucchiere.it`) |
| **Coordinate mappa** | `index.html` — blocco JSON-LD `geo` | `latitude`/`longitude` sono approssimative: verificale su Google Maps |
| **Foto** | cartella `images/` | Sostituibili con foto reali del negozio mantenendo gli stessi nomi file |
| **Recensioni** | sezione `#recensioni` | 3 recensioni reali + 3 testi coerenti: aggiorna con quelle ufficiali |

## Contatti già integrati

- **Telefono:** `tel:+393384389256`
- **WhatsApp:** `https://wa.me/393384389256` con messaggio precompilato
  *"Ciao Tommaso, vorrei prenotare un appuntamento."*
- **Indirizzo:** Via Giovanni Zappalà, 28 — 90144 Palermo (PA)
- **Google Maps:** embed senza chiave API + link "Indicazioni stradali"

## Note sulle immagini

Le foto in `images/` sono fotografie professionali da [Unsplash](https://unsplash.com)
(libere per uso commerciale, nessuna attribuzione obbligatoria), selezionate a tema
barber shop. Per il massimo impatto, consigliamo di sostituirle con foto reali del
negozio e dei lavori di Tommaso, mantenendo gli stessi nomi file e proporzioni.

## SEO

- Meta tag, Open Graph e Twitter Card
- Dati strutturati JSON-LD `HairSalon` (indirizzo, orari, telefono, rating)
- HTML semantico, immagini con `alt`, `lazy loading` e dimensioni esplicite
- Parole chiave: *barbiere Palermo, parrucchiere uomo Palermo, sfumature Palermo,
  taglio uomo Palermo, barber shop Palermo*
