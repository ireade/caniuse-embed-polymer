# `<caniuse-embed>`

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/ireade/caniuse-embed-polymer)


`<caniuse-embed>` is a Polymer Element that displays feature support data from [caniuse.com](https://caniuse.com) for multiple versions of the 10 major browsers. It is configurable, reliable, and fully responsive. This Polymer element is based on the [original JavaScript embed](https://caniuse.bitsofco.de/).

<img src="screenshot-desktop.png" alt="Desktop View of Embed" style="width: 100%;">
<img src="screenshot-mobile.png" alt="Mobile View of Embed" width="300px">

## Installation

```
bower i ireade/caniuse-embed-polymer --save
```


## Usage

There are three properties you can add to the element for configuration -

Property | Description
---------|-------------
`feature` (required) | The feature slug, retrieved from caniuse.com
`futureVersions` | The number of future browser versions to display in the embed (max 3)
`pastVersions` | The number of past browser versions to display in the embed (max 5)


## Examples

**1. Create an embed for the "SVG Effects for HTML" feature, displaying one future version and two past browser versions**


<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="caniuse-embed.html">
    <link rel="import" href="../other-element/other-element.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<caniuse-embed feature="svg-html" future-versions="1" past-versions="2"></caniuse-embed>
```


**2. Create an embed for "Viewport Units" feature, displaying only the current browser version**

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="caniuse-embed.html">
    <link rel="import" href="../other-element/other-element.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<caniuse-embed feature="viewport-units"></caniuse-embed>
```



## Copyright and Licence

- All data is from [caniuse.com](https://github.com/fyrd/caniuse), which is licenced under the [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/) license.
- The original embed is created by [Ire Aderinokun](https://twitter.com/ireaderinokun), and is licenced under the [Apache 2](http://www.apache.org/licenses/LICENSE-2.0) license.
- This Polymer element is created by [Ire Aderinokun](https://twitter.com/ireaderinokun), and is licenced under the [MIT Licence](LICENCE.md)
