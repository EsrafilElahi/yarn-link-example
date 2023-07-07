# Yarn Link Example
How to overwrite a remote package with a local development package with yarn link

### Requirement/setup:
1. Pull this repo.
2. In the demo-app, `yarn install`. Now you will have `hello-world-app` package pulled from npm, in the node_modules.
3. In the same folder, `node index.js` to see the output.

### Overwriting the same package with a local one:
1. Go to the hello-world-app and run `yarn link`.
2. Go back to demo-app and run `yarn link "hello-world-app"`.
3. Now run `node index.js` to see the different output.

### To go back to the original remote package:
1. Go to the hello-world-app and run `yarn unlink`.
2. Go back to demo-app and run `yarn unlink "hello-world-app"`.
3. Then, you will need to run `yarn install` again.
