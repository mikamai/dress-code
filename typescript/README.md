# Typescript configuration

Typescript projects configuration is done via eslint and prettier, following their recommended configuration.

## Installation

```bash
$ npm install -D eslint eslint-config-prettier eslint-plugin-prettier prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser
$ curl -o .eslintrc.js https://github.com/mikamai/dress-code/raw/master/typescript/.eslintrc.js
$ curl -o .prettierrc.js https://github.com/mikamai/dress-code/raw/master/typescript/.prettierrc.js
$ curl -O https://github.com/mikamai/dress-code/raw/master/eslint/.eslintignore
```

You also need to specify the path pattern to eslint command. Add a `lint` script in your package.json to run `eslint . --ext .ts`

## Customization

Remember to add an env property detailing your target env, so that eslint will not raise unexistent errors. For example, for a browser library, you would add:

```json
"env": {
  "browser": true
}
```

## Tests

Tests may follow different rules, and usually it would be enough to just add some overrides. There are some cases (like with mocha and jest) when you also need to set a specific env (which cannot be set in overrides). In this case, define a new `.eslintrc.js` file in your `tests` folder. It will inherit the file in the root folder by default. For example:

```json
"env": {
  "jest": true
}
```
