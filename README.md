# eslint-config-hss

Hearsay Social's base JavaScript style.

## Usage

Install this package, and eslint:

    npm install --save-dev eslint eslint-config-hss

Add this `extends` value to the root level of your `.eslintrc`:

    {
        "extends": "eslint-config-hss",
        // ...
    }

## Additional Configurations

ESLint allows you to "extend" from multiple base configurations. If you use any
of the below features, you may add these additional specialized base
configurations. Each configuration contains only the rules associated with the
given feature so you may combine them as your project demands.

### ES6

    {
        "extends": [
            "eslint-config-hss",
            "eslint-config-hss/es6"
        ],
        // ...
    }

### React

_Note_: This config requires that the package being linted have
`eslint-plugin-react@^6.7.1` installed .

    {
        "extends": [
            "eslint-config-hss",
            "eslint-config-hss/es6",
            "eslint-config-hss/react"
        ],
        // ...
    }

### Microtemplates

When linting Underscore templates with
[eslint-plugin-microtemplates](https://github.com/platinumazure/eslint-plugin-microtemplates),
some rules don't make sense. To ignore those rules, extend from this config.
Note: This config should not be applied to any js files, just html files.

    {
        "extends": [
            "eslint-config-hss/microtemplates"
        ],
        // ...
    }

## Changelog

### 5.1.0

* Add shared config for Underscore templates.

### 5.0.0

* Add shared config for React code.
* Convert `no-mixed-operators` and `no-multi-spaces` from warnings to errors.
* Disable `max-statements`.

### 4.0.0

* Begin enforcing indentation. (#7)
