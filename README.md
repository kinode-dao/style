# Kinode Style
Shared styles for Kinode apps.

## Usage

First, install Tailwind to your app's UI codebase:

```sh
yarn add tailwindcss && npx tailwindcss init
```

Then, replace your new `tailwind.config.js` file with (our config file)[./tailwind.config.js] (or modify it as necessary).

Next, add our `input.css` to the `src` folder (or modify your own to suit).

While developing, use `npx tailwindcss -i ./src/input.css -o ./src/index.css --watch` to automatically convert the Tailwind styles to CSS. 
**Note: This will overwrite any existing `index.css` file!**
