<div align="center">
  <p>
  <img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/website-project-icons/zalgo.png" height="200" alt="logo"/>
  </p>

  <p>
<h1> Awesome Zalgo </h1>
<h3> Unleash and banish the Zalgo Monster! </h3>
  </p>
<p>
  <a href="https://depfu.com/repos/Favna/awesome-zalgo"><img src="https://img.shields.io/depfu/Favna/awesome-zalgo.svg?style=flat-square" alt="Depfu" title="Depfu" /></a><!--
  --><a href="https://github.com/Favna/awesome-zalgo/blob/awesome-zalgo/LICENSE.md"><img src="https://img.shields.io/github/license/favna/awesome-zalgo.svg?style=flat-square" alt="License" title="License"></a><!--
  --><a href="https://circleci.com/gh/Favna/awesome-zalgo/tree/master"><img src="https://img.shields.io/circleci/project/github/Favna/awesome-zalgo/master.svg?style=flat-square" alt="Build Status" title="Build Status" /></a>
</p>

<p>
  <a href="https://www.npmjs.com/package/awesome-zalgo"><img src="https://img.shields.io/bundlephobia/min/awesome-zalgo.svg?style=popout-square" alt="NPM bundle size (minified)" title="NPM bundle size (minified)" /></a><!--
  --><a href="https://www.npmjs.com/package/awesome-zalgo"><img src="https://img.shields.io/bundlephobia/minzip/awesome-zalgo.svg?style=flat-square" alt="NPM bundle size (minified + gzip)" title="NPM bundle size (minified + gzip)" /></a><!--  --><a href="https://www.npmjs.com/package/awesome-zalgo"><img src="https://img.shields.io/npm/v/awesome-zalgo.svg?style=flat-square" alt="NPM Version" title="NPM Version" /></a><!--
  --><a href="https://www.npmjs.com/package/awesome-zalgo"><img src="https://img.shields.io/npm/dw/awesome-zalgo.svg?style=flat-square" alt="NPM Weekly Downloads" title="NPM Weekly Downloads" /></a><!--
  --><a href="https://www.npmjs.com/package/awesome-zalgo"><img src="https://img.shields.io/npm/dt/awesome-zalgo.svg?style=flat-square" alt="NPM Total Downloads" title="NPM Total Downloads" /></a>
</p>

<p>
  <a href="https://twitter.com/Favna_/follow"><img src="https://img.shields.io/badge/twitter-follow-brightgreen.svg?logo=twitter&colorB=1DA1F2&style=flat-square&link=https://twitter.com/Favna_/follow" alt="Follow me on Twitter" title="Follow me on Twitter" /></a><!--
  --><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XMAYCF9SDHZ34"><img src="https://img.shields.io/badge/paypal-donate-brightgreen.svg?logo=paypal&colorB=00457C&style=flat-square&link=https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XMAYCF9SDHZ34" alt="Donate with PayPal" title="Donate with PayPal" /></a><!--
  --><a href="https://www.patreon.com/bePatron?u=9336537"><img src="https://img.shields.io/badge/patreon-donate-brightgreen.svg?logo=patreon&colorB=F96854&style=flat-square&link=https://www.patreon.com/bePatron?u=9336537" alt="Become a Patron" title="Become a Patron" /></a>
</p>

<p>
  <a href="https://favna.xyz/redirect/server"><img src="https://discordapp.com/api/guilds/512303595966824458/widget.png?style=banner2" alt="Join Discord Server"/></a>
  <br/>
  <a href="https://nodei.co/npm/awesome-zalgo"><img src="https://nodei.co/npm/awesome-zalgo.png" alt="NPM Stats" title="NPM Stats" /></a>
</p>
</div>

---

This library uses the Zalgo character set from  [Acme::Zalgo](https://metacpan.org/pod/Acme::Zalgo)

# Install

Install with [yarn](https://yarnpkg.com):

```sh
$ yarn add awesome-zalgo
```

# Usage

```js
const { zalgo, banish } = require('awesome-zalgo');
// Or for babel / typescript:
// import { zalgo, banish } from 'awesome-zalgo';
// Zalgo is also available as default import. For example
// import zalgo, { banish } from 'awesome-zalgo';

// Zalgo usage
zalgo('some text')


// > ŝ̜̩͇̼̥̼́̏͢o͎͊͜ḿ̛̩̳̖͕̞̩̭ͪe͖̺̣̹̺̋̀͛̽͝ ̖͍̭͓̯̠͑͑͢t̼̪̋͌͢eͯ̋͏͖͎͍̩̭̮x̢͚̄̾̀̈ͧ̓ͩ̚t̪ͫ͝



// Banish usage
banish('ŝ̜̩͇̼̥̼́̏͢o͎͊͜ḿ̛̩̳̖͕̞̩̭ͪe͖̺̣̹̺̋̀͛̽͝ ̖͍̭͓̯̠͑͑͢t̼̪̋͌͢eͯ̋͏͖͎͍̩̭̮x̢͚̄̾̀̈ͧ̓ͩ̚t̪ͫ͝')


// > some text

// To log all the supported chars use:
const { chars } = require('awesome-zalgo/dist/chars');
console.log(chars);
```

# Documentation

<a name="ZalgoOptions"></a>

## ZalgoOptions : [<code>ZalgoOptions</code>](#ZalgoOptions)
<p>Options for the Zalgo</p>

**Kind**: Type
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| [up] | <code>boolean</code> | <p>Whether the zalgo should go up</p> |
| [middle] | <code>boolean</code> | <p>Whether the zalgo should go in the middle</p> |
| [down] | <code>boolean</code> | <p>Whether the zalgo should go downards</p> |
| [size] | <code>"mini" || "maxi" || ""</code> | <p>whethWhether the zalgo should be mini, maxi or neither<code></code></p> |

<a name="zalgo"></a>

## zalgo(text, [options]) ⇒ <code>string</code>
<p>Zalgolize any text</p>

**Kind**: function  

| Param | Type | Description |
| --- | --- | --- |
| text | <code>string</code> | <p>Input text to zalgolize</p> |
| [options] | <code><a href="#ZalgoOptions">ZalgoOptions</a></code> | <p>Options for the Zalgo</p> |

<a name="banish"></a>

## banish(purgeable) ⇒ <code>string</code>
<p>De-zalgolize any text</p>

**Kind**: function  

| Param | Type | Description |
| --- | --- | --- |
| purgeable | <code>string</code> | <p>Text to remove zalgo from</p> |

* * *

# About

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://www.github.com/favna/awesome-zalgo/issues/new).

## License

Copyright © 2019, [Favna](https://github.com/favna).
Released under the [MIT License](LICENSE.md).

## Buy me a donut

This project is open source and always will be, even if I don't get donations. That said, I know there are people out there that may still want to donate just to show their appreciation so this is for you guys. Thanks in advance!

I accept donations through PayPal, BitCoin, Ethereum and LiteCoin. You can use the buttons below to donate through your method of choice

|Donate With|QR|Address|
|:---:|:---:|:---:|
<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XMAYCF9SDHZ34"><img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/paypaldonate.png"></a>|<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XMAYCF9SDHZ34"><img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/paypalqr.png" width="128"></a>|[Donate with PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XMAYCF9SDHZ34)|
<img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/bitcoindonate.png">|<img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/bitcoinqr.png" width="128">|<a href="bitcoin:1E643TNif2MTh75rugepmXuq35Tck4TnE5?amount=0.01&label=Favna%27%20Ribbon%20Discord%20Bot">1E643TNif2MTh75rugepmXuq35Tck4TnE5</a>|
<img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/ethereumdonate.png">|<img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/ethereumqr.png" width="128">|<a href="ethereum:0xF653F666903cd8739030D2721bF01095896F5D6E?amount=0.01&label=Favna%27%20Ribbon%20Discord%20Bot">0xF653F666903cd8739030D2721bF01095896F5D6E</a>|
<img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/litecoindonate.png">|<img src="https://storage.googleapis.com/data-sunlight-146313.appspot.com/ribbon/litecoinqr.png" width="128">|<a href="litecoin:LZHvBkaJqKJRa8N7Dyu41Jd1PDBAofCik6?amount=0.01&label=Favna%27%20Ribbon%20Discord%20Bot">LZHvBkaJqKJRa8N7Dyu41Jd1PDBAofCik6</a>|
