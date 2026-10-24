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

The libraries are written in modern JavaScript with static types, using native ES modules exclusively and no compatibility layers for older environments. Dependencies are kept to a minimum, and every library can be used on its own or combined with the others.


## Runtime

TS Series is built for Node.js, with every package distributed through npm. Several libraries began on Deno, but since its official development has been discontinued, the affected repositories have been migrated in full. Committing to a single runtime and registry also keeps the release pipelines simple. Bun, the only notable alternative, was designed as a drop-in replacement for Node.js, so the restriction costs little in practice.


## License

All libraries are released under the Unlicense.
