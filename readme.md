# @esm2cjs/p-limit

This is a fork of https://github.com/sindresorhus/p-limit, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i p-limit@npm:@esm2cjs/p-limit
```

```jsonc
// package.json
"dependencies": {
    "p-limit": "npm:@esm2cjs/p-limit"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/p-limit
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/p-limit": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import pLimit from "@esm2cjs/p-limit";

// Using CommonJS require()
const pLimit = require("@esm2cjs/p-limit").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/p-limit).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/p-limit).
