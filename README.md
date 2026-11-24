# RingCalc

Webapp som regner ut hvor høye kikkertringer eller montasje en riflekikkert trenger for å klare pipe, låskasse og picatinny-skinne, og viser oppsettet visuelt.

## Funksjoner

- Anbefalt og minste ringhøyde, gap til pipe og siktehøyde (senter løp → senter kikkert)
- Plassering av kikkert og ringer fram og bak, med klaringskontroll langs hele kikkerten
- Picatinny med helning (0/3/5/10/20 MOA). Høyden måles i skinnens forkant.
- Linsedeksel utenpå objektivet
- Kikkertmaler (ZC527, K624i, NX8 4–32 og generiske) og våpenmaler (Sauer 200 STR, Sako 85 Carbon Wolf, Remington 700 SA/LA og generiske)

## Struktur

Alt ligger i `index.html` (HTML, CSS og JavaScript i én fil, ingen avhengigheter). Kikkerter og våpen legges til i listene `SCOPES` og `WEAPONS` i skriptet.

## Kjøre lokalt

Åpne `index.html` i en nettleser, eller:

```sh
npx serve .
```

## Deploy

Vercel er koblet til repoet. Hver push til `main` gir en ny produksjonsversjon, og andre brancher får en forhåndsvisning. Det er ikke noe byggetrinn, Vercel serverer filene statisk.
