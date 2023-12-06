---
sidebar_position: 5
---

`Tämä dokumentaatio on käännetty automaattisesti ja se saattaa sisältää virheitä. Älä epäröi avata Pull Requestia ehdottaaksesi muutoksia.`

# Ympäristöt

LlamaIndex tukee virallisesti tällä hetkellä NodeJS:n versioita 18 ja 20.

## NextJS-sovelluksen reititin

Jos käytät NextJS-sovelluksen reitittimen reitinkäsittelijöitä/palveluttomia funktioita, sinun tulee käyttää NodeJS-tilaa:

```js
export const runtime = "nodejs"; // oletusarvo
```

ja sinun tulee lisätä poikkeus pdf-parse:lle next.config.js-tiedostossasi

```js
// next.config.js
/** @type {import('next').NextConfig} */
const nextConfig = {
  experimental: {
    serverComponentsExternalPackages: ["pdf-parse"], // Asettaa pdf-parsen todelliseen NodeJS-tilaan NextJS-sovelluksen reitittimen kanssa
  },
};

module.exports = nextConfig;
```