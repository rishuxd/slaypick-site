# Slay Pick website

Public pages for all Slay Pick apps, hosted on Vercel (static, no build step).

- `/` : studio home, one card per game
- `/app-ads.txt` : AdMob authorised seller file. Covers every app in the AdMob account; must stay at the site root.
- `/toybox-blast/` : game page, `/toybox-blast/privacy` : privacy policy

Adding a new app: create `/<app-name>/index.html` and `/<app-name>/privacy.html` (copy Toybox Blast's and edit),
add a card on the home page, then redeploy with `npx vercel --prod` (or drag the folder onto vercel.com/new again).
Use the same site URL as the "Website" in every Play Store listing so app-ads.txt is found.
