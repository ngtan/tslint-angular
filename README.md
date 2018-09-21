# tslint-angular

## Requirements
  - [tslint](https://github.com/palantir/tslint)
  - [codelyzer](https://github.com/mgechev/codelyzer)

## Table of contents
  1. [References](#references)
  1. [Objects](#objects)
  1. [Strings](#strings)
  1. [Best Practices](#best-practices)
  1. [Stylistic](#stylistic)
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

## Objects
  1. Use property and method shorthand syntax for object literals
      ```
      "object-literal-shorthand": true
      ```

  2. Enforces consistent object literal property quote style
      ```
      "object-literal-key-quotes": [true, "consistent-as-needed"]
      ```

## Strings
  1. Use single quotes for string literals.
      ```
      "quotemark": [true, "single", "avoid-escape"]
      ```
  2. Never use `eval` on string because `eval` is dangerous as it allows arbitrary code execution with full privileges.
      ```
      "no-eval": true
      ```

## Best Practices
These rules relate to better ways of doing things to help you avoid problems

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
||[ban](https://palantir.github.io/tslint/rules/ban/)|Bans the use of specific functions (`alert`, `confirm`, `prompt`) or global methods.|
|✓|[curly](https://palantir.github.io/tslint/rules/curly/)|Enforces braces for `if`/`for`/`do`/`while` statements.|
|✓|[cyclomatic-complexity](https://palantir.github.io/tslint/rules/cyclomatic-complexity/)|Enforces a threshold of cyclomatic complexity.|
|✓|[forin](https://palantir.github.io/tslint/rules/forin/)|Requires a `for ... in` statement to be filtered with an if statement.|
|✓|[label-position](https://palantir.github.io/tslint/rules/label-position/)|Only allows labels in sensible locations.This rule only allows labels to be on `do`/`for`/`while`/`switch` statements.|
|✓|[no-arg](https://palantir.github.io/tslint/rules/no-arg/)|Disallows use of `arguments.callee`.|
|✓|[no-empty](https://palantir.github.io/tslint/rules/no-empty/)|Disallows empty blocks. Blocks with a comment inside are not considered empty.|
|✓|[no-eval](https://palantir.github.io/tslint/rules/no-eval/)|Disallows eval function invocations.|
|✓|[no-invalid-this](https://palantir.github.io/tslint/rules/no-invalid-this/)|Disallows using the this keyword outside of classes.|
||[no-magic-numbers](https://palantir.github.io/tslint/rules/no-magic-numbers/)|Disallows the use constant number values outside of variable assignments. When no list of allowed values is specified, `-1`, `0` and `1` are allowed by default.|
||[no-multi-spaces](https://github.com/buzinas/tslint-eslint-rules/blob/master/src/docs/rules/noMultiSpacesRule.md)|Dsallow use of multiple spaces|
|✓|[no-switch-case-fall-through](https://palantir.github.io/tslint/rules/no-switch-case-fall-through/)|Disallows falling through case statements.|
|✓|[no-unused-expression](https://palantir.github.io/tslint/rules/no-unused-expression/)|Disallows unused expression statements.|
|✓|[radix](https://palantir.github.io/tslint/rules/radix/)|Requires the radix parameter to be specified when calling `parseInt`|
||[switch-default](https://palantir.github.io/tslint/rules/switch-default/)|Require a `default` case in all `switch` statements.|
|✓|[triple-equals](https://palantir.github.io/tslint/rules/triple-equals/)|Requires `===` and `!==` in place of `==` and `!=`.|

## Stylistic
These rules relate to style guidelines, and are therefore quite subjective

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
|✓|[object-literal-key-quotes](https://palantir.github.io/tslint/rules/object-literal-key-quotes/)|Enforces consistent object literal property quote style.|
|✓|[quotemark](https://palantir.github.io/tslint/rules/quotemark/)|Requires single or double quotes for string literals.|
|✓|[semicolon](https://palantir.github.io/tslint/rules/semicolon/)|Enforces consistent semicolon usage at the end of every statement.|

## ECMAScript 6
These rules relate to ES6, also known as ES2015

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
|✓|[no-var-keyword](https://palantir.github.io/tslint/rules/no-var-keyword/)|Disallows usage of the `var` keyword. Use `let` or `const` instead.|
|✓|[object-literal-shorthand](https://palantir.github.io/tslint/rules/object-literal-shorthand)|Enforces/disallows use of ES6 object literal shorthand.|
|✓|[prefer-const](https://palantir.github.io/tslint/rules/prefer-const/)|Requires that variable declarations use `const` instead of `let` and `var` if possible. If a variable is only assigned to once when it is declared, it should be declared using `const`.|

## License
This project is licensed under the [MIT License](https://github.com/ngtan/tslint-angular/blob/master/LICENSE)
