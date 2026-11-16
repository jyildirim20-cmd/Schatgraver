# Schatgraver

Een kennisquiz waarin een klein gravertje steeds dieper graaft. Je krijgt een categorie (bijvoorbeeld "Noem een land in Afrika") en typt één antwoord. Hoe zeldzamer je antwoord, hoe dieper je komt: een kiezel is 10 m, een diamant 100 m. Na elke ronde zie je alle goede antwoorden, zodat je er ook van leert.

## Spelen

- **Vandaag**: iedereen krijgt elke dag dezelfde 7 categorieën. Je kunt je score kopiëren en delen.
- **Onbeperkt**: zo vaak spelen als je wilt, met steeds nieuwe categorieën.
- **Oefenen**: kies een categorie en noem er zoveel als je kunt.

## Zelf draaien

Het is één bestand zonder build-stap: open `index.html` in je browser.

## Online zetten met GitHub Pages

1. Publiceer de repository als **public**.
2. Ga op GitHub naar **Settings → Pages**.
3. Kies bij *Branch* `main` en map `/ (root)`, en klik op **Save**.
4. Na een minuutje staat het spel op `https://<gebruikersnaam>.github.io/<repo-naam>/`.

## Categorieën toevoegen

De vragen staan in `index.html` in de lijst `CATS`. Elke categorie heeft vijf niveaus, van gewoon naar zeldzaam:

```js
{t:'Naam', q:'Noem een …', a:[
  'gewoon;antwoord/alias',   // kiezel, 10 m
  '…',                       // amethist, 20 m
  '…',                       // saffier, 40 m
  '…',                       // robijn, 70 m
  '…']},                     // diamant, 100 m
```

Antwoorden scheid je met `;`, andere schrijfwijzen met `/`. Kleine typfouten worden automatisch goedgekeurd.

Hoe zeldzaam een antwoord is, is een schatting.
