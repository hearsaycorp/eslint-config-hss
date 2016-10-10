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

## Changelog

### 3.2.0

* Begin enforcing indentation. (#7)
