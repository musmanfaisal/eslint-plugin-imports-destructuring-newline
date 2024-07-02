# eslint-plugin-imports-destructuring-newline

Eslint plugin to enforce placing import and export variables on separate lines

> :heart: This project was forked from https://github.com/ruudandriessen/eslint-plugin-modules-newline <br /> Credits to the owner

## Installation

You'll first need to install [ESLint](http://eslint.org):

```
$ npm i eslint --save-dev
```
or 
```
$ yarn add eslint --dev
```

Next, install `eslint-plugin-imports-destructuring-newline`:

```
$ npm install eslint-plugin-imports-destructuring-newline --save-dev
```
or
```
$ yarn add eslint-plugin-imports-destructuring-newline --dev
```

**Note:** If you installed ESLint globally (using the `-g` flag) then you must also install `eslint-plugin-imports-destructuring-newline` globally.

## Usage

Add `eslint-plugin-imports-destructuring-newline` to the plugins section of your `.eslintrc` configuration file. You can omit the `eslint-plugin-` prefix:

```json
{
    "plugins": [
        "imports-destructuring-newline"
    ]
}
```


Then configure the rules you want to use under the rules section.

```json
{
    "rules": {
        "imports-destructuring-newline/import-declaration-newlines": ["warn", {
            "minProperties": 2
        }],
        "imports-destructuring-newline/export-declaration-newlines": "warn"
    }
}
```

## Supported Rules

* Enforce placing import variables on separate lines (import-declaration-newline). You can pass minProperties value to decide how many variables can be imported without the invokation of rule. Defaults to 2
* Enforce placing export variables on separate lines (export-declaration-newline)


