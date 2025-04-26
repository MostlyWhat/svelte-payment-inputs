# Svelte Payment Inputs

<!-- automd:badges license name="svelte-payment-inputs" color="green" github="mostlywhat/svelte-payment-inputs" -->

[![npm version](https://flat.badgen.net/npm/v/svelte-payment-inputs?color=green)](https://npmjs.com/package/svelte-payment-inputs)
[![npm downloads](https://flat.badgen.net/npm/dm/svelte-payment-inputs?color=green)](https://npmjs.com/package/svelte-payment-inputs)
[![license](https://flat.badgen.net/github/license/mostlywhat/svelte-payment-inputs?color=green)](https://github.com/mostlywhat/svelte-payment-inputs/blob/main/LICENSE)

<!-- /automd -->

Svelte Payment Inputs is a collection of unstyled payment input components for Svelte.

This is a port of [React Payment Inputs](https://github.com/medipass/react-payment-inputs) for React, which was created by [Medipass](https://github.com/medipass).

## Usage

To start using the library, install it in your project:

```bash
npm install svelte-payment-inputs
```

Use the drawer in your app.

```svelte
<script>
	import { Package } from "svelte-payment-inputs";
</script>

<Package
  name="Visa"
  number="4111 1111 1111 1111"
  expiry="12/23"
  cvc="123"
  on:change={(event) => {
    console.log(event.detail);
  }}
</Package>
```

## Documentation

The documentation is hosted on [GitHub Pages](https://mostlywhat.github.io/svelte-payment-inputs/).

## Examples

Play around with the examples on StackBlitz:

- [With scaled background](https://stackblitz.com/edit/vaul-svelte-scaled?file=src%2Froutes%2F%2Bpage.svelte)

## API Reference

TBD

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

Everything inside `src/lib` is part of the library, everything inside `src/routes` is the documentation.

## Building

To build the library:

```bash
npm run package
```

To create a production version of the documentation:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy the app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.

## Publishing

To publish the library to [npm](https://www.npmjs.com):

```bash
npm publish
```

## Testing

To run the tests, use the following command:

```bash
npm run test
```

## Roadmap

The roadmap for the project is available in the [ROADMAP.md](ROADMAP.md) file.

## Acknowledgements

TBD

## License

The svelte-payment-inputs is licensed under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) for more information.