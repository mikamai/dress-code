# ESLint configuration

We like [Airbnb styling conventions](https://github.com/airbnb/javascript), and we try to follow them, with some exceptions.

## Installation

**Non-jsx projects:**

```bash
$ npm install eslint eslint-plugin-import eslint-config-airbnb-base babel-eslint
$ curl -o .eslintrc.yml https://github.com/mikamai/dress-code/raw/master/eslint/js.eslintrc.yml
$ curl -O https://github.com/mikamai/dress-code/raw/master/eslint/.eslintignore
```

**JSX projects:**

```bash
$ npm install eslint eslint-plugin-import eslint-config-airbnb-base eslint-plugin-react eslint-plugin-jsx-a11y babel-eslint
$ curl -o .eslintrc.yml https://github.com/mikamai/dress-code/raw/master/eslint/jsx.eslintrc.yml
$ curl -O https://github.com/mikamai/dress-code/raw/master/eslint/.eslintignore
```

## Customization

Remember to add an env property detailing your target env, so that eslint will not raise unexistent errors. For example, for a browser library, you would add:

```yaml
env:
  browser: true
```

## Tests

Tests may follow different rules, and usually it would be enough to just add some overrides. There are some cases (like with mocha and jest) when you also need to set a specific env (which cannot be set in overrides). In this case, define a new `.eslintrc.yml` file in your `tests` folder. It will inherit the file in the root folder by default. For example:

```yaml
# tests/.eslintrc.yml
env:
  jest: true
```
