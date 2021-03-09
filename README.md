# TextMate grammar for Gemfile.lock files

A tmLanguage grammar for Bundler's `Gemfile.lock` files. The grammar lives in [syntaxes/gemfile-lock.tmLanguage.json](syntaxes/gemfile-lock.tmLanguage.json).

This should probably be part of a pre-existing Ruby grammar package like [atom/language-ruby](https://github.com/atom/language-ruby) or [rubyide/vscode-ruby](https://github.com/rubyide/vscode-ruby) rather than an independent project, but I needed somewhere to put the code while I was working on it so here it is.

## Tests

Tests are written using the wonderful [vscode-tmgrammar-test](https://github.com/PanAeon/vscode-tmgrammar-test) package, and live in [syntaxes/tests](syntaxes/tests).

To run the tests, you can use the "Run grammar tests" task if you're using VS Code. Otherwise, it's:

```shell
$ npm test
```

## Developing

While working on grammars I mostly use test-driven development. However, it's sometimes helpful to spin up an editor instance using the grammar to see what the syntax highlighting looks like.

This package also functions as a VS Code extension, so doing that's pretty easy. From within VS Code, just hit F5 to start an extension debugging session, then set the file type to `Gemfile.lock` (using Cmd+K M).
