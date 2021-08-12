# DENO
> Deno is a simple, modern and secure runtime for JavaScript and TypeScript that uses V8 and is built in Rust.

- Runtime for- JS/TS
- Built-in TypeScript support
- Import from URL (bye bye node_modules and central package management)
- ES6 import syntax (Bye Bye CommonJS)
- Top Level Await (what is this?)
- More compatible with browsers ( fetch, window )
- Security (flags) - Deno needs flag  permission to work
- Built-in format
- Built-in testing
- Always single executable file 

## Install Deno 

- windows 
```pwsh
iwr https://deno.land/x/install/install.ps1 -useb | iex
```
- Mac (Homebrew)
```bash
brew install deno
```
- Linux
```bash
curl -fsSL https://deno.land/x/install/install.sh | sh
```

## How to run TS/JS file in Deno

```bash
deno run index.ts
```
- Run Remote File

```bash
deno run https://deno.land/std/examples/welcome.ts
```