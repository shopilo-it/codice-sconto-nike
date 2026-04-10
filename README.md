# Cod reducere Nike — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere Nike** de pe [shopilo.it](https://shopilo.it/magazin/nike.com). Returneaza **cupoane Nike** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-nike](https://shopilo-it.github.io/codice-sconto-nike/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-nike
cd codice-sconto-nike
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Nike",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su abbigliamento sportivo",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/nike.com"
  }
]
```

## Cupoane Nike disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 20% | 20% di sconto su abbigliamento sportivo | [shopilo.it](https://shopilo.it/magazin/nike.com) |

Codurile active: **[shopilo.it/magazin/nike.com](https://shopilo.it/magazin/nike.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Nike?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/nike.com), adauga produsele in cos pe Nike, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Nike?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Nike?
Pagina [shopilo.it/magazin/nike.com](https://shopilo.it/magazin/nike.com) este actualizata zilnic cu cele mai noi cod reducere Nike, voucher Nike si cupon promotional Nike.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Nike

Nike este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/nike.com) cele mai bune cod reducere Nike, cupoane Nike verificate si voucher Nike active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-nike
```

```javascript
const { fetchCoupons } = require('codice-sconto-nike');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
