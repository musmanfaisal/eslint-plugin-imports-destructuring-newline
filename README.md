# eslint-plugin-modules-newlines

Eslint plugin to enforce placing import and export variables on separate lines

## Installation

You'll first need to install [ESLint](http://eslint.org):

```
$ npm i eslint --save-dev
```
or 
```
$ yarn add eslint --dev
```

Next, install `eslint-plugin-modules-newlines`:

```
$ npm install eslint-plugin-modules-newlines --save-dev
```
or
```
$ yarn add eslint-plugin-modules-newlines --dev
```

**Note:** If you installed ESLint globally (using the `-g` flag) then you must also install `eslint-plugin-modules-newlines` globally.

## Usage

Add `eslint-plugin-modules-newlines` to the plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
    "plugins": [
        "modules-newlines"
    ]
}
```


Then configure the rules you want to use under the rules section.

```json
{
    "rules": {
        "modules-newline/import-declaration-newlines": "warn",
        "modules-newline/import-declaration-newlines": ["warn", {
            "minProperties": 2
        }],
        "modules-newline/export-declaration-newlines": "warn"
    }
}
```

## Supported Rules

* Enforce placing import variables on separate lines (import-declaration-newline). You can pass minProperties value to decide how many variables can be imported without the invokation of rule. Defaults to 2
* Enforce placing export variables on separate lines (export-declaration-newline)

## For maintainers
AST explorer - https://astexplorer.net/#/gist/b6093767261d6a5bce76043dcea24bec/5fe761308f41936beaa30cbe7aef3a6f0283e11d




