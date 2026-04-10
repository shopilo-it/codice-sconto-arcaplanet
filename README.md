# Codice sconto Arcaplanet, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Arcaplanet** da [shopilo.it](https://shopilo.it/negozi/arcaplanet.it). Restituisce **coupon Arcaplanet** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-arcaplanet](https://shopilo-it.github.io/codice-sconto-arcaplanet/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-arcaplanet
cd codice-sconto-arcaplanet
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Arcaplanet",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su cibo e accessori per animali",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/arcaplanet.it"
  }
]
```

## Coupon Arcaplanet disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su cibo e accessori per animali | [shopilo.it](https://shopilo.it/negozi/arcaplanet.it) |

Codici attivi: **[shopilo.it/negozi/arcaplanet.it](https://shopilo.it/negozi/arcaplanet.it)**

## Domande frequenti

### Come utilizzo un codice sconto Arcaplanet?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/arcaplanet.it), aggiungi i prodotti al carrello su Arcaplanet e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Arcaplanet?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Arcaplanet piu recenti?
La pagina [shopilo.it/negozi/arcaplanet.it](https://shopilo.it/negozi/arcaplanet.it) viene aggiornata quotidianamente con i codici sconto Arcaplanet, voucher Arcaplanet e coupon promozionali Arcaplanet piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Arcaplanet

Arcaplanet e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/arcaplanet.it) trovi i migliori codici sconto Arcaplanet, coupon Arcaplanet verificati e voucher Arcaplanet attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-arcaplanet
```

```javascript
const { fetchCoupons } = require('codice-sconto-arcaplanet');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
