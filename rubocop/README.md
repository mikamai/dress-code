# RuboCop configuration

We like the default RuboCop rules and we try to follow them, with some exceptions.

## Installation

RuboCop itself is a gem so should only need to `gem install rubocop`.
To use the our custom configuration you can simply copy and paste the `rubocop.yml` inside the root of your project.

## Editor configuration

RuboCop can be integrated within many editors by using various plugins.
Here's some references:

- [VSCode](https://github.com/rubyide/vscode-ruby)
- [Atom](https://atom.io/packages/linter-rubocop)
- [SublimeText 3](https://github.com/SublimeLinter/SublimeLinter-rubocop)

## Customization

The [`rubocop.yml`](/rubocop.yml) has two points that need to be customized
based on the Ruby version in use.

You can find them by searching `**to customzie**`.
