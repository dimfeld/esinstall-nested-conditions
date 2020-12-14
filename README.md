1. npm/yarn/pnpm install
2. node index.mjs

See the error, caused by the nested condition in the `nanoid` package exports map:

```
"exports": {
  ".": {
    "browser": {
      "development": "./index.dev.js",
      "production": "./index.prod.js"
    },
    "require": "./index.cjs",
    "import": "./index.js",
    "types": "./index.d.ts"
  },
  ...
}
```
