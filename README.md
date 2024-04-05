# Kinode Style
Shared styles for Kinode apps.

## Usage

### Tailwind
Some of our apps are using Tailwind. First, install Tailwind to your app's UI codebase:

```sh
yarn add tailwindcss && npx tailwindcss init
```

Then, replace your new `tailwind.config.js` file with [our config file](./tailwind.config.js) (or modify it as necessary).

Next, add our `input.css` to the `src` folder (or modify your own to suit), and add the files in `assets` to your own `assets` folder.

While developing, use `npx tailwindcss -i ./src/input.css -o ./src/index.css --watch` to automatically convert the Tailwind styles to CSS. 
**Note: This will overwrite any existing `index.css` file!**

### UnoCSS
Some of our apps are using UnoCSS. First, install UnoCSS to your app's UI codebase:

```sh
yarn add unocss
```

Then, add our `unocss.config.ts` file to the root of your project (or modify it as necessary).

The assets will need to go in `public`.