TypeScript 2.0 introduces [a new way of to get type definitions](https://blogs.msdn.microsoft.com/typescript/2016/06/15/the-future-of-declaration-files/). Type definitions can be loaded using only `npm`. For example,

```
npm install --save @types/lodash
```

Type definitions loaded in this way can be referenced using new syntax as below:

```
/// <reference types="lodash" />
```

Type definitions can also be searched in [here](http://microsoft.github.io/TypeSearch/).

The problem with this approach is that only a number of type definitions can be found and some of them may not be up-to-date.
