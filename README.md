# MIKAMAI Dress Code

## Naming conventions

1. Repositories and git branches should be named with parameterized names, e.g. `winter-is-coming`, not `WinterIsComing`;
1. Git branches should be prefixed with the name or nickname of the branch creator;

## Mandatory in any project

1. [A language version manager](#language-version-manager);
1. [Editorconfig](#editorconfig);
1. [A linting tool](#linting-tool);

### Language version manager

For single-language projects there's no mandatory tool to use, just use the same tool across the team. For multi-language projects (e.g. Rails + React app), [asdf](https://github.com/asdf-vm/asdf) needs to be used.

*The language manager config file needs to be kept under version control.*

### Editorconfig

We use [Editorconfig](http://editorconfig.org) to keep the same coding standard across our editors. Download our [.editorconfig](.editorconfig) inside your project and ensure your editor is properly configured.

### Linting tool

For Javascript we use [ESLint](https://eslint.org/). See [our configuration](eslint/).
For Ruby we use [RuboCop](https://github.com/bbatsov/rubocop). See [our configuration](rubocop/);
