# Lists CSS

Simple CSS Grid/Subgrid based list styling.

## Installation

Using pnpm:

```bash
pnpm add @joshuabaker/lists-css
```

Using npm:

```bash
npm install @joshuabaker/lists-css
```

Using yarn:

```bash
yarn add @joshuabaker/lists-css
```

## Usage

1. Import the CSS into your project:

   ```css
   @import "@joshuabaker/lists-css";
   ```

   Or in HTML:

   ```html
   <link
     rel="stylesheet"
     href="path/to/node_modules/@joshuabaker/lists-css/index.css"
   />
   ```

2. Apply the classes to your lists:

   ```html
   <ul class="bulleted-list">
     <li>Item 1</li>
     <li>Item 2</li>
     <li>Item 3</li>
   </ul>

   <ol class="numbered-list">
     <li>Item 1</li>
     <li>Item 2</li>
     <li>Item 3</li>
   </ol>
   ```

## Customization

You can customize the width of the list markers using the `--list-marker-width` CSS custom property. The default width is `2ch`.

### Global customization:

```css
:root {
  --list-marker-width: 4ch;
}
```

### Per-list customization:

```css
.my-special-list {
  --list-marker-width: 3ch;
}
```

### Inline customization:

```html
<ul class="bulleted-list" style="--list-marker-width: 5ch;">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

## Features

- Clean, minimal styling for bulleted and numbered lists
- Customizable list marker width
- Uses CSS Grid for precise layout control
- Works with nested lists

## Browser Support

This package uses CSS Grid and CSS Custom Properties (variables). It should work in all modern browsers. For older browser support, consider using appropriate polyfills.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
