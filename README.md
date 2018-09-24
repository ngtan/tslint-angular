# tslint-angular

## Requirements
  1. [tslint](https://github.com/palantir/tslint)
  1. [codelyzer](https://github.com/mgechev/codelyzer)

## Table of contents
  1. [References](#references)
  1. [Objects](#objects)
  1. [Strings](#strings)
  1. [Possible Errors](#possible-errors)
  1. [Best Practices](#best-practices)
  1. [Variables](#variables)
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

## Possible Errors
These rules relate to possible syntax or logic errors in JavaScript code

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
|✓|[no-conditional-assignment](https://palantir.github.io/tslint/rules/no-conditional-assignment/)|Disallows any type of assignment in conditionals.|
|✓|[no-console](https://palantir.github.io/tslint/rules/no-console/)|Bans the use of specified console methods.|
|✓|[no-debugger](https://palantir.github.io/tslint/rules/no-debugger/)|Disallows `debugger` statements.|
|✓|[use-isnan](https://palantir.github.io/tslint/rules/use-isnan/)|Enforces use of the `isNaN()` function to check for `NaN` references instead of a comparison to the `NaN` constant.|
|✓|[no-unsafe-finally](https://palantir.github.io/tslint/rules/no-unsafe-finally/)|Disallows control flow statements, such as `return`, `continue`, `break` and `throws` in finally blocks.|
|✓|[trailing-comma](https://palantir.github.io/tslint/rules/trailing-comma/)|Requires or disallows trailing commas in array and object literals, destructuring assignments, function typings, named imports and exports and function parameters.|

## Best Practices
These rules relate to better ways of doing things to help you avoid problems

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
||[ban](https://palantir.github.io/tslint/rules/ban/)|Bans the use of specific functions (`alert`, `confirm`, `prompt`) or global methods.|
||[binary-expression-operand-order](https://palantir.github.io/tslint/rules/binary-expression-operand-order/)|In a binary expression, a literal should always be on the right-hand side if possible. For example, prefer `x + 1` over `1 + x`.|
|✓|[curly](https://palantir.github.io/tslint/rules/curly/)|Enforces braces for `if`/`for`/`do`/`while` statements.|
|✓|[cyclomatic-complexity](https://palantir.github.io/tslint/rules/cyclomatic-complexity/)|Enforces a threshold of cyclomatic complexity.|
|✓|[forin](https://palantir.github.io/tslint/rules/forin/)|Requires a `for ... in` statement to be filtered with an if statement.|
|✓|[label-position](https://palantir.github.io/tslint/rules/label-position/)|Only allows labels in sensible locations.This rule only allows labels to be on `do`/`for`/`while`/`switch` statements.|
|✓|[no-arg](https://palantir.github.io/tslint/rules/no-arg/)|Disallows use of `arguments.callee`.|
|✓|[no-construct](https://palantir.github.io/tslint/rules/no-construct/)|Disallows access to the constructors of `String`, `Number`, and `Boolean`.|
|✓|[no-duplicate-variable](https://palantir.github.io/tslint/rules/no-duplicate-variable/)|Disallows duplicate variable declarations in the same block scope.|
|✓|[no-empty](https://palantir.github.io/tslint/rules/no-empty/)|Disallows empty blocks. Blocks with a comment inside are not considered empty.|
|✓|[no-eval](https://palantir.github.io/tslint/rules/no-eval/)|Disallows eval function invocations.|
|✓|[no-invalid-this](https://palantir.github.io/tslint/rules/no-invalid-this/)|Disallows using the this keyword outside of classes.|
||[no-magic-numbers](https://palantir.github.io/tslint/rules/no-magic-numbers/)|Disallows the use constant number values outside of variable assignments. When no list of allowed values is specified, `-1`, `0` and `1` are allowed by default.|
|✓|[no-string-throw](https://palantir.github.io/tslint/rules/no-string-throw/)|Flags throwing plain strings or concatenations of strings.|
|✓|[no-switch-case-fall-through](https://palantir.github.io/tslint/rules/no-switch-case-fall-through/)|Disallows falling through case statements.|
|✓|[no-unused-expression](https://palantir.github.io/tslint/rules/no-unused-expression/)|Disallows unused expression statements.|
|✓|[radix](https://palantir.github.io/tslint/rules/radix/)|Requires the radix parameter to be specified when calling `parseInt`|
||[switch-default](https://palantir.github.io/tslint/rules/switch-default/)|Require a `default` case in all `switch` statements.|
|✓|[triple-equals](https://palantir.github.io/tslint/rules/triple-equals/)|Requires `===` and `!==` in place of `==` and `!=`.|

## Variables
These rules relate to variable declarations

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
|✓|[no-shadowed-variable](https://palantir.github.io/tslint/rules/no-shadowed-variable/)|Disallows shadowing variable declarations.|
||[no-unused-variable](https://palantir.github.io/tslint/rules/no-unused-variable/)|Disallows unused imports, variables, functions and private class members.|
|✓|[no-use-before-declare](https://palantir.github.io/tslint/rules/no-use-before-declare/)|Disallows usage of variables before their declaration.|

## Stylistic
These rules relate to style guidelines, and are therefore quite subjective

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
|✓|[eofline](https://palantir.github.io/tslint/rules/eofline/)|Ensures the file ends with a newline.|
|✓|[indent](https://palantir.github.io/tslint/rules/indent/)|Enforces indentation with tabs or spaces.|
|✓|[linebreak-style](https://palantir.github.io/tslint/rules/linebreak-style/)|Enforces a consistent linebreak style.|
|✓|[max-file-line-count](https://palantir.github.io/tslint/rules/max-file-line-count/)|Requires files to remain under a certain number of lines.|
|✓|[max-line-length](https://palantir.github.io/tslint/rules/max-line-length/)|Requires lines to be under a certain max length.|
|✓|[new-parens](https://palantir.github.io/tslint/rules/new-parens/)|Requires parentheses when invoking a constructor via the `new` keyword.|
|✓|[no-bitwise](https://palantir.github.io/tslint/rules/no-bitwise/)|Disallows bitwise operators.|
|✓|[no-consecutive-blank-lines](https://palantir.github.io/tslint/rules/no-consecutive-blank-lines/)|Disallows one or more blank lines in a row.|
|✓|[no-trailing-whitespace](https://palantir.github.io/tslint/rules/no-trailing-whitespace/)|Disallows trailing whitespace at the end of a line.|
|✓|[object-literal-key-quotes](https://palantir.github.io/tslint/rules/object-literal-key-quotes/)|Enforces consistent object literal property quote style.|
|✓|[one-line](https://palantir.github.io/tslint/rules/one-line/)|Requires the specified tokens to be on the same line as the expression preceding them.|
|✓|[one-variable-per-declaration](https://palantir.github.io/tslint/rules/one-variable-per-declaration/)|Disallows multiple variable definitions in the same declaration statement.|
|✓|[quotemark](https://palantir.github.io/tslint/rules/quotemark/)|Requires single or double quotes for string literals.|
|✓|[semicolon](https://palantir.github.io/tslint/rules/semicolon/)|Enforces consistent semicolon usage at the end of every statement.|
|✓|[space-before-function-paren](https://palantir.github.io/tslint/rules/space-before-function-paren/)|Require or disallow a space before function parenthesis.|
|✓|[variable-name](https://palantir.github.io/tslint/rules/variable-name/)|Checks variable names for various errors.|

## ECMAScript 6
These rules relate to ES6, also known as ES2015

| Recommended | Rule | Description |
| :---:       | :--- | :---        |
|✓|[arrow-return-shorthand](https://palantir.github.io/tslint/rules/arrow-return-shorthand/)|Suggests to convert `() => { return x; }` to `() => x`.|
|✓|[no-duplicate-super](https://palantir.github.io/tslint/rules/no-duplicate-super/)|Warns if `super()` appears twice in a constructor.|
|✓|[no-var-keyword](https://palantir.github.io/tslint/rules/no-var-keyword/)|Disallows usage of the `var` keyword. Use `let` or `const` instead.|
|✓|[object-literal-shorthand](https://palantir.github.io/tslint/rules/object-literal-shorthand)|Enforces/disallows use of ES6 object literal shorthand.|
|✓|[prefer-const](https://palantir.github.io/tslint/rules/prefer-const/)|Requires that variable declarations use `const` instead of `let` and `var` if possible. If a variable is only assigned to once when it is declared, it should be declared using `const`.|

## License
This project is licensed under the [MIT License](https://github.com/ngtan/tslint-angular/blob/master/LICENSE)
