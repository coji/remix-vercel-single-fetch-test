
Remix default template with Single Fetch enabled, vercelPreset included, and a loader in _index.tsx that just returns json({}).

When I deploy this to vercel and run it, I get the following error.


```
TypeError: headers.getSetCookie is not a function or its return value is not iterable
    at proxyResponseToResponseStub (/var/task/node_modules/.pnpm/@remix-run+server-runtime@2.9.1_typescript@5.4.5/node_modules/@remix-run/server-runtime/dist/single-fetch.js:292:25)
    at /var/task/node_modules/.pnpm/@remix-run+server-runtime@2.9.1_typescript@5.4.5/node_modules/@remix-run/server-runtime/dist/single-fetch.js:61:9
    at process.processTicksAndRejections (node:internal/process/task_queues:95:5)
    at async Promise.all (index 1)
    at async /var/task/node_modules/.pnpm/@remix-run+server-runtime@2.9.1_typescript@5.4.5/node_modules/@remix-run/server-runtime/dist/single-fetch.js:39:19
    at async callDataStrategyImpl (/var/task/node_modules/.pnpm/@remix-run+router@1.16.0/node_modules/@remix-run/router/dist/router.cjs.js:4169:17)
    at async callDataStrategy (/var/task/node_modules/.pnpm/@remix-run+router@1.16.0/node_modules/@remix-run/router/dist/router.cjs.js:3702:19)
    at async loadRouteData (/var/task/node_modules/.pnpm/@remix-run+router@1.16.0/node_modules/@remix-run/router/dist/router.cjs.js:3677:19)
    at async queryImpl (/var/task/node_modules/.pnpm/@remix-run+router@1.16.0/node_modules/@remix-run/router/dist/router.cjs.js:3522:20)
    at async Object.query (/var/task/node_modules/.pnpm/@remix-run+router@1.16.0/node_modules/@remix-run/router/dist/router.cjs.js:3416:18)
```
