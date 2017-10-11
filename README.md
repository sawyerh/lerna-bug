# Installation

```
cd project-root/ && npm install
```

# Testing the bug

**Run a working example on a non-symlinked package directory:**

```
node packages/working-test/test.js
```

This will log: "Hello, I am Bar"

**Run a non-working example on a symlinked package directory:**

```
node packages/foo-pkg/test.js
```

This will throw the following error:

```
module.js:529
    throw err;
    ^

Error: Cannot find module 'bar-pkg'
...
```