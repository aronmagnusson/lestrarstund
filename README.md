# Lestrarstund

Gagnvirkt lestrarapp á íslensku fyrir börn (7 og 9 ára). Appið er vefapp (PWA) sem virkar án nettengingar og er sett upp á spjaldtölvu með „Bæta á heimaskjá“.

## Skrár

| Skrá | Hlutverk |
|---|---|
| `index.html` | Allt appið: útlit, sögur, myndir og virkni í einni skrá |
| `sw.js` | Service worker sem geymir appið svo það virki án nets |
| `manifest.webmanifest` | Nafn, litir og tákn appsins á heimaskjá |
| `icon-*.png`, `apple-touch-icon.png` | Tákn appsins |

## Keyra á eigin tölvu

Opnaðu `index.html` beint í vafra, eða keyrðu lítinn vefþjón í möppunni (þarf fyrir offline-virknina):

```
npx serve .
```

## Útgáfa

Tengdu þetta repo við Netlify (eða GitHub Pages). Þá fer ný útgáfa sjálfkrafa í loftið í hvert sinn sem breyting er sett inn á `main`.

Þegar `index.html` breytist þarf að hækka útgáfunúmerið efst í `sw.js` (t.d. `lestrarstund-v15` → `lestrarstund-v16`), annars getur spjaldtölvan haldið áfram að sýna gömlu útgáfuna.

## Gögn

Stjörnur, nöfn, upptökur og framvinda eru vistuð í vafranum á tækinu sjálfu (localStorage og IndexedDB), ekki í þessu repoi. Notaðu „Afrit“ í foreldrasvæðinu til að taka öryggisafrit.

## Athugið

Lykilorð foreldrasvæðisins er skrifað í kóðann. Hafðu repoið **private**.
