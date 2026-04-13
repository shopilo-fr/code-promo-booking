# Code promo Booking.com, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Booking.com** depuis [shopilo.fr](https://shopilo.fr/reductions/booking.com). Renvoie les **coupons Booking.com** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-booking](https://shopilo-fr.github.io/code-promo-booking/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-booking
cd code-promo-booking
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Booking.com",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur les hotels et hebergements",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/booking.com"
  }
]
```

## Coupons Booking.com disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur les hotels et hebergements | [shopilo.fr](https://shopilo.fr/reductions/booking.com) |

Codes actifs : **[shopilo.fr/reductions/booking.com](https://shopilo.fr/reductions/booking.com)**

## Questions frequentes

### Comment utiliser un code promo Booking.com ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/booking.com), ajoutez les produits a votre panier sur Booking.com et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Booking.com ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Booking.com les plus recents ?
La page [shopilo.fr/reductions/booking.com](https://shopilo.fr/reductions/booking.com) est mise a jour quotidiennement avec les codes promo Booking.com, bons de reduction Booking.com et coupons promotionnels Booking.com les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Booking.com

Booking.com est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/booking.com), retrouvez les meilleurs codes promo Booking.com, coupons Booking.com verifies et bons de reduction Booking.com actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-booking
```

```javascript
const { fetchCoupons } = require('code-promo-booking');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
