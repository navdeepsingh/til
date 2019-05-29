# Setting up ESLint + Prettier + VSCode

- Install eslint locally or globally to project
- `eslint --init`
- .eslintrc.\* will be created and do settings as below

```js
{
parser: "babel-eslint",
  extends: ["eslint:recommended", "prettier"],
  rules: {
    quotes: ["error", "double"],
    semi: ["error", "always"],
    "prettier/prettier": [
      "error",
      {
        trailingComma: "es5",
        singleQuote: false,
        printWidth: 120
      }
    ]
  },
  plugins: ["prettier"]
}
```

- Install eslint, prettier, eslint-plugin-prettier, eslint-config-prettier, babel-eslint through npm
- Do some setting in VSCode like

```js
  // These are all my auto-save configs
  "editor.formatOnSave": true,
  // Turn it off for JS
  "[javascript]": {
    "editor.formatOnSave": true
  },
  "eslint.autoFixOnSave": true,
  "eslint.alwaysShowStatus": true
```

- Quit the VSCode and Open again.
