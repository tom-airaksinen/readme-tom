# Personal README – Tom

En enkel, statisk sida som beskriver hur jag tänker, jobbar och samarbetar bäst.

- **Live:** https://readme.tomairaksinen.se
- **Hosting:** GitHub Pages (custom domain via Loopia CNAME → `tom-airaksinen.github.io`)
- **Innehåll:** allt ligger i `index.html` (självständig, inline CSS, inga beroenden utöver Google Fonts)

## Uppdatera innehållet

Redigera `index.html`, commit:a och pusha till `main`. Pages bygger om automatiskt inom någon minut.

```sh
git add index.html
git commit -m "Uppdatera README-innehåll"
git push
```

## DNS

Subdomänen `readme.tomairaksinen.se` är en CNAME-post i Loopia som pekar på `tom-airaksinen.github.io`.
Filen `CNAME` i repot talar om för GitHub Pages vilken domän som gäller – ändra inte den utan att även uppdatera DNS.
