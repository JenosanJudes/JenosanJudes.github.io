# JudesOS – portefølje

Min portefølje, bygget som en lille computer i browseren. Hele siden er én fil: `index.html`.

## Filer

| Fil | Hvad den er |
|---|---|
| `index.html` | Selve hjemmesiden (HTML, CSS og JavaScript i én fil) |
| `README.md` | Denne vejledning |
| `LOG.md` | Arbejdsnoter: beslutninger, status og næste skridt. Ligger ikke i dette repository, men hos Jenosan |

## Se siden på din egen computer

Dobbeltklik på `index.html`. Den åbner i din browser. Der skal ikke installeres noget.

## Ret teksterne

Åbn `index.html` i IntelliJ og søg efter `const PROFIL`. Alt indhold står samlet dér:

- `om`: afsnittene i "Om mig"
- `kan` og `laerer`: kompetencerne
- `arbejde` og `uddannelse`: linjerne i "Erfaring"
- `mail`, `linkedin`, `github`: kontaktoplysninger

Ret teksten mellem anførselstegnene, gem, og genindlæs siden i browseren.

## Tilføj et projekt

Lige under `PROFIL` står `const PROJEKTER = [];`. Listen er tom, og derfor viser Projekter-mappen "Her er tomt lige nu". Tilføj et projekt sådan:

```js
const PROJEKTER = [
  {
    titel: 'Navn på projekt',
    tekst: 'Hvad det er, og hvad du lavede.',
    teknologier: ['Java', 'PostgreSQL'],
    link: 'https://github.com/JenosanJudes/projektnavn'
  }
];
```

Flere projekter adskilles med komma: `{ ... }, { ... }`.

## Læg siden på GitHub Pages

GitHub Pages er gratis hosting: GitHub viser filerne i et repository som en hjemmeside.

1. Opret et nyt, offentligt repository på GitHub. Hedder det `JenosanJudes.github.io`, bliver adressen `https://jenosanjudes.github.io`. Med et andet navn, fx `portfolio`, bliver adressen `https://jenosanjudes.github.io/portfolio`.
2. Læg `index.html` og `README.md` i repository'et (commit og push).
3. Gå til Settings → Pages i repository'et. Vælg "Deploy from a branch", branch `main` og mappen `/ (root)`. Gem.
4. Vent et par minutter. Adressen står øverst på samme side.

Hver gang du laver en ny commit og pusher til `main`, opdaterer siden sig selv.

## Eget domæne senere

Når du har købt et domæne, skriver du det ind under Settings → Pages → Custom domain og opretter de DNS-poster, GitHub viser. Siden skal ikke ændres.
