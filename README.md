# DENO
> Deno is a simple, modern and secure runtime for JavaScript and TypeScript that uses V8 and is built in Rust.

- Runtime for- JS/TS
- Built-in TypeScript support
- Import from URL (bye bye node_modules and central package management)
- ES6 import syntax (Bye Bye CommonJS)
- Top Level Await (what is this?)
- More compatible with browsers ( fetch, window )
- Security (flags) - Deno needs flag  permission to work
- Built-in format (deno fmt)
- Built-in dependency inspector (deno info) 
- Built-in testing
- Always single executable file 

## Install Deno 

- **windows (Powershell)**
```pwsh
iwr https://deno.land/x/install/install.ps1 -useb | iex
```
- **Mac (Homebrew)**
```bash
brew install deno
```
- **Linux**
```bash
curl -fsSL https://deno.land/x/install/install.sh | sh
```
- More way to install , see [deno.land](https://deno.land/)

## Updating Deno

```pwsh
deno upgrade
```

## How to run TS/JS file in Deno

```bash
deno run index.ts
```
- **To Run Remote File**

```bash
deno run https://deno.land/std/examples/welcome.ts
```
## NodeJS vs Deno

- No npm
    - It uses modules referenced as URLs or file paths.
- No Package.json
- All async actions in Deno return a promise. Thus Deno provides different APIs than Node
- Deno requires explicit permissions for file, network, and environment access.

- Deno always dies on uncaught errors.
- Deno uses "ES Modules" and does not support require(). Third party modules are imported via URLs:

```ts
import * as log from "https://deno.land/std@0.105.0/log/mod.ts";
```

## Other key behaviors 
- Fetch and cache remote code upon first execution, and never update it until the code is run with the --reload flag. (So, this will still work on an airplane.)
- Modules/files loaded from remote URLs are intended to be immutable and cacheable.

