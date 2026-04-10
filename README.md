# Codice sconto Myprotein, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Myprotein** da [shopilo.it](https://shopilo.it/negozi/myprotein.it). Restituisce **coupon Myprotein** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-myprotein](https://shopilo-it.github.io/codice-sconto-myprotein/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-myprotein
cd codice-sconto-myprotein
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Myprotein",
    "code": "SHOPILO30",
    "discount": "30%",
    "description": "30% di sconto su integratori e proteine",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/myprotein.it"
  }
]
```

## Coupon Myprotein disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 30% | 30% di sconto su integratori e proteine | [shopilo.it](https://shopilo.it/negozi/myprotein.it) |

Codici attivi: **[shopilo.it/negozi/myprotein.it](https://shopilo.it/negozi/myprotein.it)**

## Domande frequenti

### Come utilizzo un codice sconto Myprotein?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/myprotein.it), aggiungi i prodotti al carrello su Myprotein e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Myprotein?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Myprotein piu recenti?
La pagina [shopilo.it/negozi/myprotein.it](https://shopilo.it/negozi/myprotein.it) viene aggiornata quotidianamente con i codici sconto Myprotein, voucher Myprotein e coupon promozionali Myprotein piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Myprotein

Myprotein e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/myprotein.it) trovi i migliori codici sconto Myprotein, coupon Myprotein verificati e voucher Myprotein attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-myprotein
```

```javascript
const { fetchCoupons } = require('codice-sconto-myprotein');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
