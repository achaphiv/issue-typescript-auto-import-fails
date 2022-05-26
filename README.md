# Issue

See: [Issue](https://github.com/microsoft/TypeScript/issues/45637)

Open [index.ts](./index.ts) and attempt to import this in VSCode.

Nothing happens and the following output will be shown in `Log (extension Host)`:

```none
[2022-05-26 03:44:28.559] [exthost] [error] Error: <semantic> TypeScript Server Error (4.6.3)
Debug Failure. False expression.
Error: Debug Failure. False expression.
    at getCompletionEntryCodeActionsAndSourceDisplay (/opt/visual-studio-code/resources/app/extensions/node_modules/typescript/lib/tsserver.js:130376:22)
    at Object.getCompletionEntryDetails (/opt/visual-studio-code/resources/app/extensions/node_modules/typescript/lib/tsserver.js:130314:30)
    at Object.getCompletionEntryDetails (/opt/visual-studio-code/resources/app/extensions/node_modules/typescript/lib/tsserver.js:161877:35)
    at /opt/visual-studio-code/resources/app/extensions/node_modules/typescript/lib/tsserver.js:173451:57
    at Object.mapDefined (/opt/visual-studio-code/resources/app/extensions/node_modules/typescript/lib/tsserver.js:605:30)
    at IpcIOSession.Session.getCompletionEntryDetails (/opt/visual-studio-code/resources/app/extensions/node_modules/typescript/lib/tsserver.js:173449:33)
```
