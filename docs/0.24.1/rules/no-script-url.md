---
title: Rule no-script-url
layout: doc
---
<!-- Note: No pull requests accepted for this file. See README.md in the root directory for details. -->
# Disallow Script URLs (no-script-url)

Using `javascript:` urls is considered by some as a form of eval. Script passed after javascript: has to be parsed and evaluated by the browser the same way that it does eval.

## Rule Details

The following patterns are considered warnings:

```js
location.href = "javascript:void(0)";
```

## Compatibility

* **JSHint**: This rule corresponds to `scripturl` rule of JSHint.

## Further Reading

* [What is the matter with script-targeted URLs?](http://stackoverflow.com/questions/13497971/what-is-the-matter-with-script-targeted-urls)

## Version

This rule was introduced in ESLint 0.0.9.

## Resources

* [Rule source](https://github.com/eslint/eslint/tree/master/lib/rules/no-script-url.js)
* [Documentation source](https://github.com/eslint/eslint/tree/master/docs/rules/no-script-url.md)
