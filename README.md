# MIKAMAI Dress Code

## Mandatory in any project

- [MIKAMAI Dress Code](#mikamai-dress-code)
  - [Mandatory in any project](#mandatory-in-any-project)
    - [Language version manager](#language-version-manager)
    - [Editorconfig](#editorconfig)
    - [Linting tool](#linting-tool)

### Language version manager

For single-language projects there's no mandatory tool to use, just use the same tool across the team. For multi-language projects (e.g. Rails + React app), [asdf](https://github.com/asdf-vm/asdf) needs to be used.

*The language manager config file needs to be kept under version control.*

### Editorconfig

We use [Editorconfig](http://editorconfig.org) to keep the same coding standard across our editors. Download our [.editorconfig](.editorconfig) inside your project and ensure your editor is properly configured.

### Linting tool

For Javascript we use [ESLint](https://eslint.org/). See [our configuration](eslint/).
For Typescript projects we use [ESLint](https://eslint.org/) and [Prettier](https://prettier.io/). See [our configuration](typescript/).
For Ruby we use [RuboCop](https://github.com/bbatsov/rubocop). See [our configuration](rubocop/);
