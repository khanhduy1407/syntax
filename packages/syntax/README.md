# NKDuy Syntax

## Usage

```sh
npm i @nkduy/syntax
# yarn add @nkduy/syntax
```

```js
const syntax = require('@nkduy/syntax')

syntax
  .getHighlighter({
    theme: 'nord'
  })
  .then(highlighter => {
    console.log(highlighter.codeToHtml(`console.log('syntax');`, { lang: 'js' }))
  })

// <pre class="nkd-syntax" style="background-color: #2e3440"><code>
//   <!-- Highlighted Code -->
// </code></pre>
```

```html
<script src="https://unpkg.com/@nkduy/syntax"></script>
<script>
  syntax
    .getHighlighter({
      theme: 'nord'
    })
    .then(highlighter => {
      const code = highlighter.codeToHtml(`console.log('syntax');`, { lang: 'js' })
      document.getElementById('output').innerHTML = code
    })
</script>
```

- [Themes](./docs/themes.md)
- [Languages](./docs/languages.md)

## License

MIT
