# Personal README – Tom

En enkel, statisk sida som beskriver hur jag tänker, jobbar och samarbetar bäst.

- **Live:** https://readme.tomairaksinen.se
- **Hosting:** GitHub Pages (custom domain via Loopia CNAME → `tom-airaksinen.github.io`)
- **Innehåll:** allt ligger i `index.html` (självständig, inline CSS, inga beroenden utöver Google Fonts)

## Uppdatera innehållet

Redigera `index.html`, commit:a och pusha till `main`. Pages bygger om automatiskt inom någon minut.

```sh
git pull --rebase        # hämta ev. CNAME-commits som GitHub lagt till automatiskt
# redigera index.html ...
git add index.html
git commit -m "Uppdatera README-innehall"
git push
```

> **Obs:** GitHub lägger ibland till egna "Create/Delete CNAME"-commits direkt på remote
> (händer när custom-domän/HTTPS konfigureras). Kör därför alltid `git pull --rebase` först –
> annars nekas din push med "remote contains work that you do not have locally".
> Undvik `!` och oavslutade `"` i commit-meddelanden (zsh klagar med `event not found` / `dquote>`).

## DNS

Subdomänen `readme.tomairaksinen.se` är en CNAME-post i Loopia som pekar på `tom-airaksinen.github.io`.
Filen `CNAME` i repot talar om för GitHub Pages vilken domän som gäller – ändra inte den utan att även uppdatera DNS.
