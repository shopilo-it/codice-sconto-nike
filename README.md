# Codice sconto Nike, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Nike** da [shopilo.it](https://shopilo.it/negozi/nike.com). Restituisce **coupon Nike** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-nike](https://shopilo-it.github.io/codice-sconto-nike/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-nike
cd codice-sconto-nike
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Nike",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su abbigliamento sportivo",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/nike.com"
  }
]
```

## Coupon Nike disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su abbigliamento sportivo | [shopilo.it](https://shopilo.it/negozi/nike.com) |

Codici attivi: **[shopilo.it/negozi/nike.com](https://shopilo.it/negozi/nike.com)**

## Domande frequenti

### Come utilizzo un codice sconto Nike?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/nike.com), aggiungi i prodotti al carrello su Nike e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Nike?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Nike piu recenti?
La pagina [shopilo.it/negozi/nike.com](https://shopilo.it/negozi/nike.com) viene aggiornata quotidianamente con i codici sconto Nike, voucher Nike e coupon promozionali Nike piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Nike

Nike e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/nike.com) trovi i migliori codici sconto Nike, coupon Nike verificati e voucher Nike attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-nike
```

```javascript
const { fetchCoupons } = require('codice-sconto-nike');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
