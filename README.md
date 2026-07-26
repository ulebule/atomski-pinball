# ATOMSKI PINBALL

Retro flipper v brskalniku, po vzoru **Atari Video Pinball (1980)**.
Vse je v eni sami datoteki `index.html` — brez knjižnic, brez gradnje,
brez omrežnih klicev. Dvojni klik in igraš.

## Igraj

Odpri `index.html` v brskalniku, ali obišči objavljeno stran (GitHub Pages).

## Kontrole

| Tipka | Dejanje |
|---|---|
| `◀` `▶` | levi / desni zaklopec |
| `▼` ali `presledek` | napni in sproži žogo |
| `Z` / `X` | nudge (sunek v mizo) |
| `Enter` | start / nova igra |
| `M` | zvok vklop / izklop |

Na dotik: leva in desna tretjina zaslona sta zaklopca, spodnji srednji del
je vzmet, gumb `↯` zgoraj desno je nudge.

## Miza

- **trije okrogli odbijači** — 100 točk
- **Atari diamant** v sredini — 500 točk; štirje zadetki prinesejo **dodatno žogo**
- **A-T-A-R-I** rolloverji na vrhu — 300 točk vsak, vseh pet prižganih da
  **5000 točk** in poveča množitelj (do x5)
- **vrtavka** ob levem robu — 10 točk na vrtljaj
- **prožilca** (slingshota) nad zaklopcema — 50 točk
- **tilt**: trije sunki zapored zaklenejo zaklopca do izgube žoge

Tri žoge na igro. Rekord in lestvica najboljših desetih se shranjujeta
lokalno v brskalniku (`localStorage`) — vezano na napravo in brskalnik.

## Jeziki

Vmesnik zazna jezik naprave; z gumbom zgoraj levo se vrti med
slovenščino, angleščino, nemščino, italijanščino in francoščino.
