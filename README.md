# @yutengjing/biome-config

## Install

```shell
pnpm install -D @yutengjing/biome-config
```

> [!NOTE] > `@biomejs/biome` is the peerDependencies

## Config

### Add to biome.json

```json
{
  "$schema": "./node_modules/@biomejs/biome/configuration_schema.json",
  "extends": ["./node_modules/@yutengjing/biome-config/biome.json"]
}
```

### VSCode settings

Add following to `.vscode/settings.json`:

```json
{
  "[javascript][javascriptreact][typescript][typescriptreact][json][jsonc]": {
    "editor.defaultFormatter": "biomejs.biome"
  },
  "editor.codeActionsOnSave": {
    "quickfix.biome": "explicit",
    "source.organizeImports.biome": "explicit"
  }
}
```

> [!NOTE]
> Ensure you had already installed [biome VSCode extension](https://marketplace.visualstudio.com/items?itemName=biomejs.biome)

## Related

- [@yutengjing/eslint-config](https://github.com/tjx666/eslint-config/tree/main)
- [@yutengjing/stylelint-config](https://github.com/tjx666/stylelint-config/tree/main)
- [@yutengjing/prettier-config](https://github.com/tjx666/prettier-config/tree/main)
- [@yutengjing/tsconfig](https://github.com/tjx666/tsconfig/tree/main)
