This repo reproduces the following bug:

When installed via NPM, a subpackage installed via a local file reference will not have its own dependencies installed.

To reproduce the bug :

Fails with NPM

```
cd app-package && npm i
node index.js # >> Return error
```

Success with Yarn

```
cd app-package && yarn
node index.js # >> Returns ok
```
