# Repo for `@messageformat/runtime/messages` issue

This repo contains files that demonstrate a problem when importing `@messageformat/runtime/messages` in TypeScript.

## Steps to reproduce

```cirru
npm install
npx tsc
```

## Expected result

- `test1.js` and `test2.js` files are built correctly and without any error.

## Actual result

- Build of `test2.js` fails with error:
  ```markdown
  test2.ts:1:20 - error TS7016: Could not find a declaration file for module '@messageformat/runtime/messages'. 'C:/Users/katem/src/ization/repro--messageformat-runtime-messages/node_modules/@messageformat/runtime/messages.js' implicitly has an 'any' type.
    Try `npm i --save-dev @types/messageformat__runtime` if it exists or add a new declaration (.d.ts) file containing `declare module '@messageformat/runtime/messages';`

  1 import * as M from '@messageformat/runtime/messages';
                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  ```
