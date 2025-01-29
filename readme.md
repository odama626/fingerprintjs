<p align="center">
  <img src="resources/logo_dark.svg" alt="FingerprintJS logo" width="312px" />
</p>

FingerprintJS is a browser fingerprinting library that queries browser attributes and computes a hashed visitor identifier from them. Unlike cookies and local storage, a fingerprint stays the same in incognito/private mode and even when browser data is purged.

This repository is a fork of FingerprintJS that was originally licensed under the MIT License. It has been rereleased as `@sparkstone/fingerprintjs` under the same MIT license.

## Installation

You can install `@sparkstone/fingerprintjs` using your preferred package manager:

### pnpm

```sh
pnpm add @sparkstone/fingerprintjs
```

### npm

```sh
npm install @sparkstone/fingerprintjs
```

### yarn

```sh
yarn add @sparkstone/fingerprintjs
```

## Quick start

Here is a basic TypeScript example of how to use FingerprintJS:

```typescript
import FingerprintJS from '@sparkstone/fingerprintjs'

// Initialize the agent at application startup.
const fp = await FingerprintJS.load()

// Get the visitor identifier when you need it.
const result = await fp.get()

// This is the visitor identifier:
console.log(result.visitorId)
```

📕 [Full documentation](docs/api.md)

## Migrating from v2

-   [Migration guide](docs/migrating_v2_v3.md)

## Version policy

See the compatibility policy for the API and visitor identifiers in the [version policy guide](docs/version_policy.md).

## Supported browsers

The library supports all popular browsers.
See more details and learn how to run the library in old browsers in the [browser support guide](docs/browser_support.md).

## Where to get support

Using [Issues](https://github.com/odama626/fingerprintjs/issues) and [Discussions](https://github.com/odama626/fingerprintjs/discussions) publicly will help the open-source community and other users with similar issues.

## Contributing

See the [contribution guidelines](contributing.md) to learn how to start a playground, test, and build.
