# Modern Accessibilty CSS Reset

A style reset specifically aimed at accessibility that embraces modern CSS features to help start your project without accessibility errors.

> This is not a CSS reset to replace normalise.css or other CSS resets. This is a reset that is specifically aimed at accessibility.

## Features

- Designed for cascade layers by using the modern `@layer` directive.
- Improved readability for text and headings.
- Proper resets for form elements.
- Accessible, consistent focus outlines.
- `.visually-hidden` and `.sr-only` class baked in.
- Reduced motion media query baked in.

### Usage

Install and import the package (requires a bundler):

```sh
npm install a11y-reset
```

Then, I'd recommend you import this reset into the first layer after your existing reset. You can predefine your layers as the first thing in your stylesheet:

```css
@layer reset, a11y-reset, some, other, layers;
```

Then import the reset:

```css
@import 'a11y-reset' layer(a11y-reset);
```

#### Another CSS reset?

CSS resets like normalise.css create sensible defaults and eliminate browser bugs. Use one of these and you get a consistent base across all browsers.

**a11y-reset** takes a different and complimentary approach. Its aim is to prevent accessibility errors and provide sensible defaults for accessibility. It's not a replacement for a CSS reset, but a complimentary reset.
