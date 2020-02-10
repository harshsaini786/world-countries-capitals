#### Want to contribute to open source? check issues [here.](https://github.com/bhatvikrant/world-countries-capitals/issues)

# world-countries-capitals

<!-- ![](https://img.shields.io/github/forks/bhatvikrant/world-countries-capitals?style=social)

<!-- ![](https://img.shields.io/github/stars/bhatvikrant/world-countries-capitals?style=social) -->

#### A simple [NPM](https://www.npmjs.com/package/world-countries-capitals) package to get capitals, currency, native language etc. of all the countries in the world

![world-countries-capitals](assets/world-countries-capitals.gif)

[Website](https://bhatvikrant.github.io/world-countries-capitals/)

## Getting started

[![NPM](https://nodei.co/npm/world-countries-capitals.png?compact=true)](https://nodei.co/npm/world-countries-capitals/)

## Installation

[![NPM INSTALL](http://img.shields.io/badge/npm-install-blue.svg?style=for-the-badge&logo=npm)](https://docs.npmjs.com/getting-started/installing-npm-packages-locally) [![NODE JS](http://img.shields.io/badge/Node-JS-teal.svg?style=for-the-badge&logo=node.js)](https://nodejs.org/en/) [![NODE JS](https://img.shields.io/npm/v/world-countries-capitals?logo=npm&label=world-countries-capitals&style=for-the-badge)](https://www.npmjs.com/package/world-countries-capitals)

This is a [Node.js](https://nodejs.org/en/) module available through the
[npm registry](https://www.npmjs.com/).

Before using, [download and install Node.js](https://nodejs.org/en/download/).

Installation is done using the
**[`npm install`](https://docs.npmjs.com/getting-started/installing-npm-packages-locally)** command:

```bash
$ npm i world-countries-capitals --save
```

---

## Importing

```javascript
const wcc = require("world-countries-capitals");
```

---

## Usage

-   **getAllCountryDetails()** This method returns an **array of objects** of all countries, each containing **country**, **capital**, **currency** and **native_language**.

```json
    [
        {
            "country": "afghanistan",
            "capital": "kabul",
            "currency": "afghani",
            "native_language": ["dari persian", "pashto"]
        },
        {
            "country": "albania",
            "capital": "tirane",
            "currency": "lek",
            "native_language": ["albanian"]
        },

        ...
    ]
```

---

-   **getAllCountries()** This method returns an **array** of **names** of all countries.

```javascript
    [
        'afghanistan',
        'albania',
        'algeria',
        'andorra',
        'angola',
        'antigua & Barbuda',
        'argentina',
        'armenia',
        'australia',
        'austria',
        'azerbaijan',
        ...
    ]
```

---

-   **getCountiesByLanguage(languageSpoken)** This method returns an **array of objects**, each containing **country**, **capital**, **currency** and **native_language** sorted by the _languageSpoken_.

Response for languageSpoken = 'Hindi'

```javascript
[
    {
        country: "fiji",
        capital: "suva",
        currency: "fijian dollar",
        native_language: ["english", "bau fijian", "hindi"]
    },
    {
        country: "india",
        capital: "new delhi",
        currency: "indian rupee",
        native_language: ["hindi", "english"]
    }
];
```

---

-   **getCountryDetailsByName(countryName)** This method returns an **array of objects**, each containing **country**, **capital**, **currency** and **native_language** sorted by the _name of the country_ .

Response for countryName = 'india'

```javascript
[
    {
        country: "india",
        capital: "new delhi",
        currency: "indian rupee",
        native_language: ["hindi", "english"]
    }
];
```

---

-   **getCountryDetailsByCapital(capital)** This method returns an **array of objects**, each containing **country**, **capital**, **currency** and **native_language** sorted by the _capital_ .

Response for capital = 'delhi'

```javascript
[
    {
        country: "india",
        capital: "new delhi",
        currency: "indian rupee",
        native_language: ["hindi", "english"]
    }
];
```

---

-   **getRandomCountry()** This method returns a random country everytime.

```bash
» node app.js
tuvalu

» node app.js
bhutan

» node app.js
saudi arabia
```

##### where app.js is the file containing the function call.

---

-   **getNRandomCountriesData(n)** This method returns an array having **n** random country objects, each object containing **country**, **capital**, **currency** and **native_language**.

Response for n = 3

```javascript
[
    {
        country: "burundi",
        capital: "bujumbura",
        currency: "burundi franc",
        native_language: ["kirundi", "french"]
    },
    {
        country: "palau",
        capital: "melekeok",
        currency: "united states dollar",
        native_language: ["english", "palauan"]
    },
    {
        country: "dominican republic",
        capital: "santo domingo",
        currency: "dominican peso",
        native_language: ["spanish"]
    }
];
```

---

# Examples

## #1

```javascript
const wcc = require("world-countries-capitals");

console.log(wcc.getRandomCountry());
```

## #2

```javascript
const wcc = require("world-countries-capitals");

console.log(wcc.getNRandomCountriesData(3));
```

## #3

```javascript
const wcc = require("world-countries-capitals");

console.log(wcc.getCountryDetailsByCapital("delhi"));
```

#### in this example the parameter (capital), which has to be a string can be a written in uppercase/lowercase etc. the response will be the same.

## #4

```javascript
const wcc = require("world-countries-capitals");

console.log(wcc.getCountryDetailsByName("India"));
```

#### in this example the parameter (countryName), which has to be a string can be a written in uppercase/lowercase etc. the response will be the same.

## #5

```javascript
const wcc = require("world-countries-capitals");

console.log(wcc.getCountiesByLanguage("hindi"));
```

#### in this example the parameter (languageSpoken), which has to be a string can be a written in uppercase/lowercase etc. the response will be the same.

## #6

```javascript
const wcc = require("world-countries-capitals");

console.log(wcc.getAllCountryDetails());
```

## #7

```javascript
const wcc = require("world-countries-capitals");

console.log(wcc.getAllCountries());
```

---

# Want to contribute?

<!-- [![Open Source Love](https://badges.frapsoft.com/os/v3/open-source-175x29.png?v=103)](https://github.com/bhatvikrant/world-countries-capitals/issues) -->

> Please check issues **[here](https://github.com/bhatvikrant/world-countries-capitals/issues)**!

---

## License

![GitHub license](https://img.shields.io/github/license/bhatvikrant/world-countries-capitals.svg?style=for-the-badge&logo=github)

---

## Let's get connected

[![Twitter Follow](https://img.shields.io/twitter/follow/vikrantbhat1022.svg?style=for-the-badge&logo=twitter)](https://twitter.com/vikrantbhat1022)

[![GitHub followers](https://img.shields.io/github/followers/bhatvikrant.svg?label=Follow&style=for-the-badge&logo=github)](https://github.com/bhatvikrant/)

[![LinkedIn](https://img.shields.io/static/v1.svg?label=connect&message=@vikrantbhat&color=success&logo=linkedin&style=for-the-badge&logoColor=white&colorA=blue)](https://www.linkedin.com/in/vikrant-bhat-2b6221189/)

<hr>

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://github.com/bhatvikrant/world-countries-capitals) [![forthebadge](https://forthebadge.com/images/badges/made-with-javascript.svg)](https://github.com/bhatvikrant/world-countries-capitals) [![forthebadge](https://forthebadge.com/images/badges/makes-people-smile.svg)](https://github.com/bhatvikrant/world-countries-capitals) [![forthebadge](https://forthebadge.com/images/badges/check-it-out.svg)](https://github.com/bhatvikrant/world-countries-capitals)
