# `@hedger/eslint-config`

This repository contains ESLint configuration presets for my projects.

## Usage

Install the packages

```bash
pnpm add -D eslint @hedger/eslint-config
```

Configure `.eslintrc.json`

```json
{
  "extends": "@hedger"
}
```

Setup script in `package.json`

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

Configure VS Code auto fix

```json
{
  "prettier.enable": false,
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## Overriding rules

In `eslintrc.json`

```json
{
  "extends": "@hedger",
  "rules": {
    // your rules...
  }
}
```

## Credits

Huge thanks to [@antfu](https://github.com/antfu) for his work on [@antfu/eslint-config](https://github.com/antfu/eslint-config/) which this repository is based on.

## License

This repository is licensed under the [MIT license](./LICENSE.md).
