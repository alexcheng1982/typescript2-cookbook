# TypeScript 2 Cookbook

As a software developer who uses both Java and JavaScript for a long time, I realize that strong type checking is a crucial part in software development. The compiler can help us to find more bugs in the very early stage of development. When developing JavaScript code, it's always driving me crazy when finding out that a bug was caused by a typo or missing a newly added argument in some old code. That's why I think [TypeScript](https://www.typescriptlang.org/) is a good fit for web application development. However, TypeScript is still very young and it's hard to find answers for some common problems. You may also find out that some important features is missing in current version of TypeScript. But I think learning TypeScript is a good investment in the long run.

This book is about the current beta version of TypeScript - TypeScript 2.0. The goal is to include cookbook style recipes for common tasks when using TypeScript 2.

### Install

To install current TypeScript 2.0 beta version, use `npm install typescript@beta`. To install next 2.1 version, use `npm install typescript@next`.

### Upgrade Visual Studio Code to use a newer version of TypeScript

[Visual Studio Code](https://code.visualstudio.com) is a good tool for editing TypeScript files. To upgrade Visual Studio Code to use a newer version of TypeScript, see [here](https://code.visualstudio.com/docs/languages/typescript#_using-newer-typescript-versions) for the guide.

The recommended approach is to open `settings.json` file in `.vscode` directory and update `typescript.tsdk` to `node_modules/typescript/lib`. Then you can always use `npm` to install newer version of TypeScript for current project.