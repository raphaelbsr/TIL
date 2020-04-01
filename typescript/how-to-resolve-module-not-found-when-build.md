# Today I Learn

### How to resolve module not found error when run typescript project

If we set path alias in tsconfig.json, we should got a module not found error at runtime, to solve this we need to install module-alias lib and define the paths in \_moduleAliases options in pakage.json.

```javascript
// 1 - Install module-alias
yarn add module-alias

// 2 - add _moduleAliases in package.json
"_moduleAliases": {
    "@modules": "dist/modules",
    "@services": "dist/services"
}

// 3 - add import 'module-alias/register'; at the top of project startup file
import 'module-alias/register';

```

### Links

[Reference](https://dev.to/larswaechter/path-aliases-with-typescript-in-nodejs-4353)
