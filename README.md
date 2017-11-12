# eslint-config-ohar [![travis][travis-image]][travis-url] [![npm][npm-image]][npm-url] [![downloads][downloads-image]][downloads-url] [![javascript style guide][standard-image]][standard-url]

#### An ESLint [Shareable Config](http://eslint.org/docs/developer-guide/shareable-configs) for [JavaScript Standard Style](http://standardjs.com)

Based on [eslint-config-standard](https://github.com/standard/eslint-config-standard) with some minor improvements.

## Why fork `eslint-config-standard`?

Standard is not bad, but there were some problems here.

* Not possible to align code by colon to form text-based vertical columns
* Trailing commas disabled. [Nik Graf wrote an article](https://medium.com/@nikgraf/why-you-should-enforce-dangling-commas-for-multiline-statements-d034c98e36f8) about why it should be not enabled, but even forced to,

## Install

### NPM

```bash
npm install -D eslint-config-ohar
```
### Yarn

```bash
yarn add -D eslint-config-ohar
```

## Usage

Shareable configs are designed to work with the `extends` feature of `.eslintrc` files.
You can learn more about
[Shareable Configs](http://eslint.org/docs/developer-guide/shareable-configs) on the
official ESLint website.

To use the JavaScript Standard Style shareable config, first run this:

### NPM

```bash
npm install -D eslint-config-ohar eslint-plugin-standard eslint-plugin-promise eslint-plugin-import eslint-plugin-node
```

### Yarn

```bash
yarn add -D eslint-config-ohar eslint-plugin-standard eslint-plugin-promise eslint-plugin-import eslint-plugin-node
```

Then, add this to your .eslintrc file:

```
{
  "extends": "standard"
}
```

*Note: We omitted the `eslint-config-` prefix since it is automatically assumed by ESLint.*

You can override settings from the shareable config by adding them directly into your
`.eslintrc` file.

### Looking for something easier than this?

The easiest way to use JavaScript Standard Style to check your code is to use the
[`standard`](http://standardjs.com) package. This comes with a global
Node command line program (`standard`) that you can run or add to your `npm test` script
to quickly check your style.


## Learn more

For the full listing of rules, editor plugins, FAQs, and more, visit the main
[JavaScript Standard Style repo](http://standardjs.com).

## License

MIT. Copyright (c) [Feross Aboukhadijeh](http://feross.org), [Pavel Lysenko](http://ohar.name).
