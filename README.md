# Formatieve assignment 3

Dit is de repository die hoort bij de formatieve assignment 3 van het vak TICT-SV2FEP2-20.

## De applicatie: Fantasy Weapons Store

De 'Fantasy Weapons Store' is een applicatie waarmee je fantasy weapons kan aanschaffen. Op de overzichtspagina vind je alle weapons. Je kan filteren op de categorieën, types en varianten waarin je geïnteresseerd bent. Wanneer je op een weapon klikt, navigeer je naar de productpagina van dit weapon. Op deze pagina vind je informatie over het weapon, en kan je het toevoegen aan (of verwijderen uit) je cart. Op de cart pagina vind je een overzicht van de producten die je hebt toegevoegd aan je cart. Ook kan je hier aanpassingen doen aan de producten in je cart.

## Setup

```sh
git clone https://github.com/TICT-SV2FEP2-20/formatieve-assignment-2.git
cd formatieve-assignment-2
```

### Dependencies

Deze repository maakt gebruik van [NodeJS](http://nodejs.org/) en NPM.

### Usage

- Ga naar de juiste directory: `cd assignment-2`
- Installeer de node modules met `npm i`
- run `npm start`

## Directory and file structure

### Components

De applicatie is opgebouwd uit drie pagina's, zoals hierboven beschreven: de overzichtspagina (`index.html`), de productpagina (`product.html`) en de cart (`cart.html`). Deze pagina's bestaan uit een component (geprefixed met `view-`) die je kan vinden in de directory `components`.

Neem de `components` directory door om te zien uit welke componenten de applicatie nog meer is opgebouwd. Neem de tijd om te kijken waar de componenten gebruikt worden, wat hun verantwoordelijkheid is, en hoe verschillende componenten met elkaar communiceren.

### Data

Deze directory bevat alle data (de verschillende weapons en categorieen) in `.json` formaat.

### Utils

Deze directory bevat een aantal utility functions, die door meerdere componenten gebruikt kunnen worden.

- `get-data.js`: voor het ophalen van de data. De data wordt teruggeven als een promise met json content.
- `cart-js`: deze file bevat een aantal functies die betrekking hebben op de cart, zoals het toevoegen en verwijderen uit de cart. De functies maken gebruik van [localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) om de data lokaal in de browser op te slaan.
- `get-selected-option-values.js`: voor het teruggeven van de geselecteerde filter.

### Assets

De `assets` directory bevat alle afbeeldingen die in de applicatie gebruikt worden.

### `app.js`

Het `AppRoot` component is het root component, het 'entry point', van de applicatie. Het bevat alle andere views/components.

### `styles.css`

Deze file bevat de algemene styling van de applicatie. Het is styling die niet specifiek is voor een component.

### Overige files

Een aantal bestanden, zoals `package.json`, `package-lock.json`, `main.js` en `serve.json` zijn nodig voor het serveren van de applicatie. Bekijk deze files om te zien wat er gebeurt. Ze zijn niet nodig voor het maken van de assignments.