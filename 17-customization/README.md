# Customization

Tailwind customization is configured in `tailwind.config.js`.

## Basic Structure

```js
module.exports = {
  content: [],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

## How It Works

The `theme` section defines the values available to your utilities.

The `extend` section adds new values without replacing the default theme.

If you define values directly inside `theme`, they replace the corresponding default values.

## Example

```js
tailwind.config = {
  theme: {
    screens: {
      sm: "550px",
      md: "800px",
      lg: "1200px",
      xl: "1440px",
    },
    extend: {
      colors: {
        primary: "#FF5733",
        secondary: "#FFFC33",
      },
      spacing: {
        128: "32rem",
      },
      borderRadius: {
        "4xl": "2rem",
      },
    },
  },
};
```

## Tailwind v3 Docs

- Configuration: https://v3.tailwindcss.com/docs/configuration
