## PHP Standards Recommendations
### psr-1 Basic Coding Standard
*   Files MUST use only **<?php** or **<?=** tags.
*   Files MUST use only **UTF-8** without **BOM** for PHP code.
*   Files SHOULD either declare symbols(classes, functions, constants, etc.) or
cause side-effects(e.g.generate output, change .ini settings, etc.) but SHOULD NOT do both
*   Namespaces and classed MUST follow an "autoloading" PSR:[PSR-0, PSR-4].
*   Class names MUST be declared in **StudlyCaps**.
*   Class constants MUST be declared in upper case with underscore separators.
*   Method names MUST be declared in **camelCase**.
- - -
### psr-2 Coding Style Guide
*   Code MUST follow a "coding style guide" PSR [PSR-1].
*   Code MUST use 4 spaces for indenting, not tabs.
*   There MUST NOT be a hard limit on line length, the soft limit MUST be 120
characters; lines SHOULD be 80 characters or less.
*   There MUST be one blank line after the `namespace` declaration, and MUST
be one blank line after the block of `use` declarations.
*   Opening braces for classes or methods MUST go on the next line, the closing
braces MUST go on the next after the body.
*   Visibility MUST be declared on all methods and properties, `abstract` and
`final` MUST be declared before visibility, `static` MUST be declared after
Visibility.
*   Control structure keywords MUST MUST have one spaces after them; method and
function calls MUST not.
*   Opening braces for control structures MUST go on the same line, the closing
braces MUST go on the next line after the body.
*   Opening parentheses for control structures MUST NOT have a space after them,
and closing parentheses for control structures MUST NOT have a space before.
- - -
### psr-3 Logger Interface

### psr-7 Http message interfaces
