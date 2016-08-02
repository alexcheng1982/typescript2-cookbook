It's highly possible that you cannot find type definitions for certain modules. Maybe the module you are using is not very popular and no one contributes type definitions for it.

To use these modules, we can use the new [wildcard module names](https://github.com/Microsoft/TypeScript/wiki/What's-new-in-TypeScript#wildcard-character-in-module-names) in TypeScript 2.0.

We can add a file `declarations.d.ts` in app directory to declare those modules. You only need to write one line to declare the module.

```
declare module 'react-css-modules';
```

Then you can use the standard TypeScript way to import the module.

```
import * as CSSModules from 'react-css-modules';
```

The `declarations.d.ts` file should be added to `files` section of `tsconfig.json` file.
