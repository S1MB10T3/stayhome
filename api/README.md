<a href="https://www.buymeacoffee.com/covidapi/shop" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-black.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
# Join our Server!
[![Discord server](https://discordapp.com/api/guilds/689535536934813823/embed.png?style=banner4)](https://discord.gg/EvbMshU)

# API
API for Current cases and more stuff about COVID-19 or the Novel Coronavirus Strain
https://corona.lmao.ninja/

# Recommended by Postman
NovelCovid API is recommended by Postman [here](https://covid-19-apis.postman.com/)

# Documentation
NovelCovid/API Documentation can be found [here](https://docs.corona.lmao-xd.wtf)

## Loading and using our NPM Package

We suggest you load the module via `require`, considering ES modules in Node.js are not yet stable.

```js
const covid = require('novelcovid');
```

## Documentation
Executing a method will return a [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise). The examples here utilise [async/await](https://javascript.info/async-await) to access the data.

```js
// Declare the package
const covid = require('novelcovid');

// Now we create a async/await
(async () => {

    // Now we await it.
    let all = await covid.getAll();

    // Make sure you return it, this usually implies if you are using this inside a function.
    // Use \n to break lines.
    return console.log(`Cases: ${all.cases}\nDeaths: ${all.deaths}\nRecovered: ${all.recovered}`)
})()
```

#### Sorting the data.

Some [methods](https://www.npmjs.com/package/covidtracker#methods) can be sorted.

```js
const covid = require('novelcovid');

(async () => {
    let sortedCountries = await covid.getCountry({sort: 'recovered'});
    return console.log(sortedCountries);

    let sortedStates = await covid.getState({sort: 'deaths'});
    return console.log(sortedStates);
})();
```

#### Filtering for a specific country/state.
```js
const covid = require('novelcovid');

(async () => {
   // Specific Country
   let specificCountry = await covid.getCountry({country: 'United States'});
   return console.log(specificCountry);
   
   // Specific State
   let specificState = await covid.getState({state: 'New York'});
   return console.log(specificCountry);
})();
```

**Note**
Since `data.updated` returns milliseconds, you can do `new Date(data.updated)` as it returns an **ISO Date**

You can read more about **new Date()** [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

> For further support, you can join our discord server! More Tutorials can be found there too!
> https://discord.gg/EvbMshU

### Sources: 
> https://www.worldometers.info/coronavirus/

> https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/EliteDaMyth"><img src="https://avatars2.githubusercontent.com/u/28687771?v=4" width="100px;" alt=""/><br /><sub><b>EliteDaMyth</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/commits?author=EliteDaMyth" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/ebwinters"><img src="https://avatars0.githubusercontent.com/u/4297028?v=4" width="100px;" alt=""/><br /><sub><b>Ethan Winters</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/issues?q=author%3Aebwinters" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/dicedtomatoreal"><img src="https://avatars0.githubusercontent.com/u/35403473?v=4" width="100px;" alt=""/><br /><sub><b>dicedtomato</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/commits?author=dicedtomatoreal" title="Code">💻</a></td>
    <td align="center"><a href="https://404discord.xyz/"><img src="https://avatars0.githubusercontent.com/u/41652412?v=4" width="100px;" alt=""/><br /><sub><b>apollyon600</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/commits?author=apollyon600" title="Documentation">📖</a></td>
    <td align="center"><a href="https://jshelley.uk"><img src="https://avatars0.githubusercontent.com/u/22616014?v=4" width="100px;" alt=""/><br /><sub><b>James Shelley</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/pulls?q=is%3Apr+reviewed-by%3AJamesShelley" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="http://RyanHarlow.com"><img src="https://avatars2.githubusercontent.com/u/42226213?v=4" width="100px;" alt=""/><br /><sub><b>Ryan Harlow</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/issues?q=author%3ARyanHarlow" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/alitas"><img src="https://avatars1.githubusercontent.com/u/1144691?v=4" width="100px;" alt=""/><br /><sub><b>Ali Tas</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/issues?q=author%3Aalitas" title="Bug reports">🐛</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/buster95"><img src="https://avatars0.githubusercontent.com/u/15637669?v=4" width="100px;" alt=""/><br /><sub><b>Walter Corrales</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/commits?author=buster95" title="Code">💻</a></td>
    <td align="center"><a href="https://AhmadAwais.com"><img src="https://avatars1.githubusercontent.com/u/960133?v=4" width="100px;" alt=""/><br /><sub><b>Ahmad Awais ⚡️</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/commits?author=ahmadawais" title="Documentation">📖</a></td>
    <td align="center"><a href="https://discord.gg/rk7cVyk"><img src="https://avatars1.githubusercontent.com/u/39545629?v=4" width="100px;" alt=""/><br /><sub><b>MrAugu</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/issues?q=author%3AMrAugu" title="Bug reports">🐛</a></td>
    <td align="center"><a href="http://chroventer.github.io"><img src="https://avatars2.githubusercontent.com/u/34645569?v=4" width="100px;" alt=""/><br /><sub><b>Ayyan Lewis</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/issues?q=author%3Achroventer" title="Bug reports">🐛</a></td>
    <td align="center"><a href="http://bensommer.co.uk"><img src="https://avatars0.githubusercontent.com/u/39101651?v=4" width="100px;" alt=""/><br /><sub><b>Ben Sommer</b></sub></a><br /><a href="https://github.com/NovelCOVID/API/issues?q=author%3Abenjamin-sommer" title="Bug reports">🐛</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
