# tslint-angular

## Requirements
  - [tslint](https://github.com/palantir/tslint)
  - [codelyzer](https://github.com/mgechev/codelyzer)

## Table of contents
  1. [References](#references)
  1. [ECMAScript 6](#ecmascript-6)

## References
  1. Use `const` instead of `let` and `var` if a variable is only assigned to once when it is declared.
      ```
      "prefer-const": true
      ```

  2. Use `let` instead of `var` if a variable is reassigned.
      ```
      "no-var-keyword": true
      ```


## ECMAScript 6
These rules relate to ES6, also known as ES2015

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
|✓|[no-var-keyword](https://palantir.github.io/tslint/rules/no-var-keyword/)|Disallows usage of the `var` keyword. Use `let` or `const` instead.|
|✓|[prefer-const](https://palantir.github.io/tslint/rules/prefer-const/)|Requires that variable declarations use `const` instead of `let` and `var` if possible. If a variable is only assigned to once when it is declared, it should be declared using `const`.|

## License
This project is licensed under the [MIT License](https://github.com/ngtan/tslint-angular/blob/master/LICENSE)
