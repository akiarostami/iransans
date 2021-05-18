# IRANSans

The CSS and web font files to easily self-host the “IRANSans” font. Please visit the [github repo](https://github.com/akiarostami/iransans) to view more details on this package.

## Installation

We assumes you are using a bundler, such as Webpack, to load in CSS. Solutions like [CRA](https://create-react-app.dev/), [Gatsby](https://www.gatsbyjs.org/) and [Next.js](https://nextjs.org/) are prebuilt examples that are compatible.

```javascript
yarn add @akiarostami/iransans // npm install @akiarostami/iransans
```

Then within your app entry file or site component, import it in. For example in Gatsby, you could choose to import it into a layout template (`layout.js`), page component (`index.js`), or `gatsby-browser.js`.

```javascript
import '@akiarostami/iransans'; // Defaults to weight 400.
```

This repo  allows you to select weights and even individual styles, allowing you to cut down on payload sizes to the last byte.

```javascript
import '@akiarostami/iransans/500.css'; // Weight 500.
import '@akiarostami/iransans/900-italic.css'; // Italic variant.
```

Alternatively, the same solutions could be imported via SCSS.

```scss
@import '~@akiarostami/iransans/index.css'; // Weight 400.
@import '~@akiarostami/iransans/300-italic.css';
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
import '@akiarostami/iransans/500-pn.css'; // Weight 500 with normal style.
```

## Licensing

This source code is free to use. However, to use IranSans you have to obtain the rights from [FontIran](https://fontiran.com).
