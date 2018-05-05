# TSLint Airbnb Style Guide config

> A [TSLint config](https://palantir.github.io/tslint/usage/tslint-json/) for [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
highly opinionated and customizable


This project is inspirrated by [tslint-config-airbnb](https://github.com/progre/tslint-config-airbnb).

The main difference is that this project also includes more rules provided not only by eslint but also by TsLint to strict even more the validations.


## Installation

```sh
npm i -S @webdev-tools/tslint-airbnb-styleguide
```

## Usage

You can remove all rules on your `tslint.json` and only set:

```json
{
  "extends": "tslint-airbnb-styleguide"
}
```

## Usage on Angular CLI projects

Angular has its own [Style Guide](https://angular.io/guide/styleguide) and requires additional rules:

```json
{
  "extends": "tslint-airbnb-styleguide",
  "rulesDirectory": [
    "node_modules/codelyzer"
  ],
  "rules": {
    "directive-selector": [
      true,
      "attribute",
      ["app"],
      "camelCase"
    ],
    "component-selector": [
      true,
      "element",
      ["app"],
      "kebab-case"
    ],
    "no-output-on-prefix": true,
    "use-input-property-decorator": true,
    "use-output-property-decorator": true,
    "use-host-property-decorator": true,
    "no-input-rename": true,
    "no-output-rename": true,
    "use-life-cycle-interface": true,
    "use-pipe-transform-interface": true,
    "component-class-suffix": true,
    "directive-class-suffix": true,
    "no-unused-variable": true
  }
}
```


### Rules Available

* [tslint](https://www.npmjs.com/package/tslint)
* [tslint-consistent-codestyle](https://www.npmjs.com/package/tslint-consistent-codestyle)
* [tslint-eslint-rules](https://www.npmjs.com/package/tslint-eslint-rules)
* [tslint-microsoft-contrib](https://www.npmjs.com/package/tslint-microsoft-contrib)


## License

Apache 2.0
