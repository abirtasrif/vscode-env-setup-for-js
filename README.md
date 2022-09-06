# Setup VScode environment with for javaScript programming

1. Make sure nodejs is installed.
2. Install yarn globally `npm install -g yarn`
3. Install below extensions for vscode (No need if already setup)-

- [eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [path-autocomplete](https://marketplace.visualstudio.com/items?itemName=ionutvmi.path-autocomplete)

4. Select "LF" instead of "CRLF" from editor bottom ribbon.
5. Add below lines inside settings.json ,put a comma `,` at the end of last line inside `}` and add below

```
  "[javascript]": {
    "editor.formatOnSave": false,
    "editor.defaultFormatter": null
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.organizeImports": true
  },
  "eslint.alwaysShowStatus": true

```

6. download and put the files `.eslintrc.json` and `yarn.lock` to your project. run `yarn install` in terminal.
