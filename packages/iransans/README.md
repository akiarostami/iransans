# PersianFonts IRANSans

The CSS and web font files to easily self-host the “IRANSans” font. Please visit the main [Fontsource monorepo](https://github.com/akiarostami/PersianFont) to view more details on this package.

## Installation

PersianFonts assumes you are using a bundler, such as Webpack, to load in CSS. Solutions like [CRA](https://create-react-app.dev/), [Gatsby](https://www.gatsbyjs.org/) and [Next.js](https://nextjs.org/) are prebuilt examples that are compatible.

```javascript
yarn add @persianfonts/iransans // npm install @persianfonts/iransans
```

Then within your app entry file or site component, import it in. For example in Gatsby, you could choose to import it into a layout template (`layout.js`), page component (`index.js`), or `gatsby-browser.js`.

```javascript
import '@persianfonts/iransans'; // Defaults to weight 400.
```

PersianFonts allows you to select weights and even individual styles, allowing you to cut down on payload sizes to the last byte! Utilizing the CSS unicode-range selector, all language subsets are accounted for.

```javascript
import '@persianfonts/iransans/500.css'; // Weight 500.
import '@persianfonts/iransans/900-italic.css'; // Italic variant.
```

Alternatively, the same solutions could be imported via SCSS!

```scss
@import '~@persianfonts/iransans/index.css'; // Weight 400.
@import '~@persianfonts/iransans/300-italic.css';
```

Finally, you can reference the font name in a CSS stylesheet, CSS Module, or CSS-in-JS.

```css
body {
  font-family: 'IRANSans';
}
```

## Additional Options

In the case you need to Persian Numerals, you can add "-pn" to the name of the css file:

```javascript
import '@persianfonts/iransans/500-ns.css'; // Weight 500 with normal style.
```

## Licensing

It is important to always read the license for every font that you use.
Most of the fonts in the collection are from FontIran and you have to obtain the rights from their website.

[FontIran](https://fontiran.com)
