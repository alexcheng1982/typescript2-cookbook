Tools like [tsd](https://github.com/DefinitelyTyped/tsd) and [typings](https://github.com/typings/typings) can be used to load type definitions from community-driven repositories, like [DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped). I recommend to use typings.

## typings

Use `npm install typings -g` to install typings CLI. Then type definitions can be searched and installed.

```
typings search --name react

typings install debug --save
```

Metadata of type definitions installed by typings is kept in `typings.json` file. Actual type definitions files are installed into `typings` directory. Both `typings.json` and `typings` directory should be maintained in source code repository.

## For TypeScript

To use type definitions installed by typings, add an entry of `typings/index.d.ts` in `files` section of `tsconfig.json` file.

```
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "sourceMap": true,
    "jsx": "react",
    "lib": ["dom", "es5", "es2015.promise"]
  },
  "compileOnSave": false,
  "files": [
    "typings/index.d.ts"
  ]
}
```
