# Pokémon Story — HTML en CSS leren

## Doel van het project
Een website met drie pagina's om HTML, afbeeldingen, navigatielinks, tabellen, lijsten en CSS te oefenen. De bron bevat een verhaal over het ontstaan van Pokémon, een beperkte tabel en een overzicht van Pokémon-types.

## Bestanden en hun functie

| Pad | Wat gebeurt er? |
| --- | --- |
| `index.html` | Startpagina met titels, paragrafen en achtergrondinformatie. |
| `pokemons.html` | HTML-tabel met vijf Pokémon en hun eigenschappen. |
| `types.html` | Geordende lijst met de achttien Pokémon-types en bijhorende iconen. |
| `styles.css` | Algemene opmaak: lettertype, maximale breedte, links, banner, tabel, afbeeldingen. |
| `images/` | Lokale afbeeldingen (`001.png` enz.) en type-iconen (`.svg`). |

## Belangrijke HTML-concepten

- **`<head>`** bevat metadata en koppelingen naar CSS; **`<body>`** bevat de zichtbare pagina.
- **`<a href="types.html">`** navigeert naar een andere pagina in dezelfde map.
- **`<img src="images/001.png" alt="Bulbasaur">`** verwijst naar een relatief bestandspad. De `alt`-tekst beschrijft de afbeelding voor schermlezers.
- **`<table>`** bevat rijen (**`<tr>`**), kopcellen (**`<th>`**) en gewone cellen (**`<td>`**). **`<thead>`** en **`<tbody>`** scheiden de tabelkop van de gegevens.
- **`<ol>`** bouwt een genummerde lijst. Elk type is een **`<li>`**.
- **`class="table-image"`** wordt in CSS geselecteerd met `.table-image`. **`id="banner"`** wordt geselecteerd met `#banner`.
- **`max-width: 980px`** begrenst de inhoudsbreedte. **`margin-left/right: auto`** centreert de pagina.
- **`overflow-x: auto`** laat een brede tabel horizontaal schuiven op smalle schermen.

## Bevindingen en aanpassingen

- In `pokemons.html` stonden `<div>`-elementen midden in `<tr>`-rijen. Dat is geen geldige tabelstructuur. Die omhulsels zijn weggehaald.
- De afbeeldingspaden zijn behouden en er zijn beschrijvende `alt`-teksten toegevoegd.
- Bij Charmander en Charmeleon wees het pictogram naar `fire.svg`, maar er stond verkeerdelijk 'grass' als tekst. Dat is hersteld naar 'fire'.
- In `types.html` ontbraken Dark, Steel en Fairy, terwijl de bijbehorende SVG-bestanden al in `images/` aanwezig waren. De lijst bevat nu achttien types.
- De laatste afsluitende `</div>` in `types.html` is aangevuld.
- CSS maakt de Pokémon-tabel beter bruikbaar op een klein scherm.

## Nog onafgewerkt / te controleren

- De tabel toont **vijf Pokémon**. De map `images/` bevat méér afbeeldingen, maar de oorspronkelijke opdracht vermeldt niet hoeveel tabelrijen vereist zijn. Daarom zijn er geen extra Pokémon verzonnen of toegevoegd.
- De oorspronkelijke HP- en Speed-waarden zijn overgenomen, **niet** vergeleken met een officiële Pokédex. Controleer ze nog als nauwkeurige Pokémon-statistieken deel uitmaken van de opdracht.
- De drie pagina's zijn statisch nagelezen; klik de links en controleer de afbeeldingen en weergave op Android of in een browser.

## Zelf oefenen

1. Voeg één Pokémonrij toe aan de tabel. Welke zeven cellen moet je invullen?
2. Verander de achtergrondkleur van de navigatiebalk in CSS.
3. Verander het uiterlijk van de type-iconen zonder de HTML aan te passen.
4. Leg in je eigen woorden het verschil uit tussen een **klasse** en een **id**.

**Opmerking:** deze documentatie is afgeleid uit de aanwezige broncode, niet uit een afzonderlijke leerkrachtopdracht.
