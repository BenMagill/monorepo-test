# Monorepo example
See [npm workspaces](https://docs.npmjs.com/cli/v7/using-npm/workspaces) for general info.

## Questions to resolve 
- how to build and deploy a single service?
- how to maintain versions of packages used or must it always be the latest?
- can packages be built into the node_modules or is it just a symlink?

## How it works
When running `npm i` (or `npm ci`), it will build the packages included in the `packages` directory and they will be added to the node_modules directory for use.

## Adding a package 
Run `npm init -w ./packages/NAME` or just create a folder and add it to the root `package.json`.