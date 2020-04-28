# Nucleum stylelint Config

A sharable [stylelint][stylelint] configuration for [Nucleum].

Extends: [stylelint-config-recommended], [stylelint-config-property-sort-order-smacss] and [stylelint-scss].

[stylelint]: https://stylelint.io/
[Nucleum]: https://github.com/CosAnca/nucleum
[stylelint-config-recommended]: https://github.com/stylelint/stylelint-config-recommended
[stylelint-config-property-sort-order-smacss]: https://github.com/cahamilton/stylelint-config-property-sort-order-smacss
[stylelint-scss]: https://github.com/kristerkari/stylelint-scss

Turns on additional rules to enforce common stylistic conventions found within the ITCSS architectural pattern:

To see the rules that this config uses, please read the [config](/index.js) itself.

## Installation

If using **npm**, run:

```bash
npm install stylelint-config-nucleum --save-dev
```

If using **Yarn**, run:

```bash
yarn add stylelint-config-nucleum --dev
```

## Usage

Set your [stylelint configuration][stylelint-configuration] to:

```json
{
  "extends": "stylelint-config-nucleum"
}
```

You can override rules from the shared configuration, by setting your
own values within the `rules` property:

```json
{
  "extends": "stylelint-config-nucleum",
  "rules": {
    "string-quotes": "single"
  }
}
```

You can also turn a rule off, by setting the value of the rule to `null`:

```json
{
  "extends": "stylelint-config-nucleum",
  "rules": {
    "string-quotes": null
  }
}
```

[stylelint-configuration]: https://stylelint.io/user-guide/configuration/

### Atom integration

stylelint can be integrated into [Atom][atom] so that you will be alerted of
any warnings and errors inline, while you work.

Install the [linter][linter] and [linter-stylelint][linter-stylelint] packages
using Atom’s package manager or enter this into your terminal:

```bash
apm install linter linter-stylelint
```

[atom]: https://atom.io/
[linter]: https://atom.io/packages/linter
[linter-stylelint]: https://atom.io/packages/linter-stylelint

## License

Nucleum stylelint Config is copyright (c) 2020 Cos Anca. It is free software, and may be redistributed under the terms specified in the [LICENSE] file.

[LICENSE]: /LICENSE.md

## About

Nucleum stylelint Config is maintained by [Cos Anca](https://github.com/CosAnca).

I love open source software! See [my other projects][community].

[community]: https://github.com/CosAnca
