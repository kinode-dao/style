# Kinode Style
Shared styles for Kinode apps.

## Usage

### Tailwind
Some of our apps are using Tailwind. First, install Tailwind to your app's UI codebase:

```sh
yarn add tailwindcss && npx tailwindcss init
```

Then, replace your new `tailwind.config.js` file with [our config file](./tailwind.config.js) (or modify it as necessary).

Next, add our `input.css` (NOT `index.css`) to the `src` folder (or modify your own to suit), and add the files in `assets` to your own `assets` folder.

While developing, use `tailwindcss` to automatically convert the Tailwind styles to CSS:

```sh
# Note: This will overwrite any existing `index.css` file!
npx tailwindcss -i ./src/input.css -o ./src/index.css --watch 
```

### UnoCSS
Some of our apps are using UnoCSS. First, install UnoCSS to your app's UI codebase:

```sh
yarn add unocss
```

Next, add our `index.css` (NOT `input.css`) to the `src` folder (or modify your own to suit) *and rename it to `index.css`*, and add the files in `assets` to your ***`public`*** folder.

Then, add our `unocss.config.ts` file to the root of your project (or modify it as necessary).

Finally, modify your `vite.config.ts`:

```ts
import UnoCSS from 'unocss/vite'

export default defineConfig({
  plugins: [
    react(),
    UnoCSS()
  ],
  // ...
})
```