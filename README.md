# POOL BTC mining pool dataset

Fees, payout schemes, minimum payouts and stratum addresses for 25 crypto mining pools, 20 of which mine Bitcoin. Maintained by [POOL BTC](https://pool-btc.com/), an independent comparison of Bitcoin mining pools.

Updated: 2026-11-02. Live version: https://pool-btc.com/dataset/en/

## Files

- `pools.csv`: one row per pool
- `pools.json`: same data with metadata (source, license, update date)

## Fields

| Field | Meaning |
|---|---|
| `id`, `name`, `website` | pool identifier, name, official site |
| `coins` | coins the pool mines |
| `btc` | `true` if the pool mines Bitcoin |
| `solo` | `true` if solo mining is offered |
| `algorithm` | supported algorithms |
| `payout_scheme` | FPPS, PPS+, PPLNS and so on |
| `fee_percent` | pool fee, percent |
| `min_payout` | minimum payout |
| `fee_source`, `fee_verified` | page the fee was taken from and the date it was checked |
| `stratum`, `worker_format`, `stratum_source` | connection addresses, worker name format, source page |

Each fee links to the pool's own page. Pools change terms, so check `fee_verified` and the source before relying on a number.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Free to use, share and adapt, including commercially, with attribution:

> Data: POOL BTC (https://pool-btc.com/)
