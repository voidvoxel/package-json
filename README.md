# `@voidvoxel/package-json`

[![Known Vulnerabilities](https://snyk.io/test/github/voidvoxel/package-json/badge.svg)](https://snyk.io/test/github/voidvoxel/package-json)

Programmatically access and modify `package.json` files.

## Installation

```sh
npm i @voidvoxel/package-json
```

## Usage

```js
// Import the package.
import PackageJSON from "@voidvoxel/package-json";
/* OR */
const PackageJSON = require("@voidvoxel/package-json");

// Read a `package.json` file.
const packageJSONPath = "./package.json";
const packageJSON = PackageJSON.readFileSync(packageJSONPath);

// Change some values.
packageJSON.name = "example-package";
packageJSON.version = "4.2.0";

// Add a dependency to the package.
packageName.addDependency("moment");

// Save our changes to the file.
PackageJSON.writeFileSync(
    packageJSONPath,
    packageJSON
);
```
