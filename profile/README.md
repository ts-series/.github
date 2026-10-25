# TS Series

TS Series is a collection of small, focused TypeScript libraries and command-line tools for building websites and web applications. The libraries cover both the server and the browser, keep their dependencies to a minimum and follow a consistent design, so they can be combined freely or used on their own.


## Libraries

| Library | Description |
| ------- | ----------- |
| [app-server](https://github.com/ts-series/app-server) | Page routing with partial loading and TypeScript client modules without a build step, on Hono |
| [case](https://github.com/ts-series/case) | Conversion between casing styles for identifiers and text |
| [dom-factories](https://github.com/ts-series/dom-factories) | Factory functions for creating and composing HTML elements in the browser |
| [factories](https://github.com/ts-series/factories) | Generation of static HTML on the server |
| [hashing](https://github.com/ts-series/hashing) | Fast, allocation-free MurmurHash3 implementation |
| [lite-client](https://github.com/ts-series/lite-client) | Driver-agnostic SQLite ORM with type-safe queries that stay close to SQL |
| [settings](https://github.com/ts-series/settings) | YAML settings and translations, loaded at runtime or generated as typed code |
| [smake](https://github.com/ts-series/smake) | CLI tool that generates SQLite databases and the matching lite-client ORM classes |

Every library is published to the official npm registry under the `@ts-series` scope, for instance:

```bash
pnpm install @ts-series/lite-client
```

All code is written in modern JavaScript with static types, using native ES modules exclusively and no compatibility layers for older environments.


## Runtime

TS Series supports Node.js only, with every package distributed through npm. Earlier versions targeted Deno and remain on JSR, but they are no longer updated since the official development of Deno has been discontinued.

Committing to a single runtime and registry keeps the release pipelines simple.


## Security

Most supply chain risks in the Node.js ecosystem come from deep dependency trees, because a single compromised package can reach every project that uses it. TS Series avoids this by keeping every library simple and free of dependencies. Where a dependency is unavoidable, it has no dependencies itself and builds on web standards. The code in a project therefore stays small and easy to audit, which makes the libraries suitable for security-critical areas.


### Reporting a Vulnerability

Vulnerabilities are reported privately using the "Report a vulnerability" button on the Security tab of the affected repository. Public issues are not suitable, as a publicly disclosed vulnerability can be exploited before a fix exists and before users have had time to update. Reports are acknowledged within 7 days.


### Supported Versions

Only the latest release of each library receives security fixes.


## Licensing

All software is dual licensed and available under both 0BSD and Apache License 2.0. Contributions fall under the same terms, including a patent license, as described in [CONTRIBUTING.md](https://github.com/ts-series/.github/blob/main/CONTRIBUTING.md).
