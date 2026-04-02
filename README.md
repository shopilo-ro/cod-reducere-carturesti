# Cod reducere Carturesti — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Carturesti** de pe [shopilo.ro](https://shopilo.ro/magazin/carturesti.ro). Returneaza **cupoane Carturesti** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-carturesti](https://shopilo-ro.github.io/cod-reducere-carturesti/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-carturesti
cd cod-reducere-carturesti
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Carturesti",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la toate produsele in stoc",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/carturesti.ro"
  }
]
```

## Cupoane Carturesti disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la toate produsele in stoc | [shopilo.ro](https://shopilo.ro/magazin/carturesti.ro) |

Codurile active: **[shopilo.ro/magazin/carturesti.ro](https://shopilo.ro/magazin/carturesti.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Carturesti?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/carturesti.ro), adauga produsele in cos pe Carturesti, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Carturesti?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Carturesti?
Pagina [shopilo.ro/magazin/carturesti.ro](https://shopilo.ro/magazin/carturesti.ro) este actualizata zilnic cu cele mai noi cod reducere Carturesti, voucher Carturesti si cupon promotional Carturesti.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Carturesti

Carturesti este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/carturesti.ro) cele mai bune cod reducere Carturesti, cupoane Carturesti verificate si voucher Carturesti active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-carturesti
```

```javascript
const { fetchCoupons } = require('cod-reducere-carturesti');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
