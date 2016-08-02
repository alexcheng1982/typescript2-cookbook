Type definitions play the most import role in TypeScript. That's why it's call TypeScript. For your own TypeScript code, you just need to use `import` statement to import the modules, TypeScript compiler can find the type definitions.

The hard part is for third-party JavaScript modules and legacy JavaScript code. You may have seen the error `Error TS2307: Cannot find module 'module-name'.`  many times.

* [`tsd` and `typings`](tsd_typings.md)
* [@types](types.md)
* [When no type definitions](no_type_definitions.md)

# Summary

At the moment of writing, it's recommended to use `typings` tool to load type definitions and use wildcard module names for those modules without type definitions.
