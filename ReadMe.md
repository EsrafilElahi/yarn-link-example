# Yarn Link Example
How to overwrite a remote package with a local development package with yarn link

### Requirement/setup:
1. Pull this repo.
2. In the demo folder, `yarn install`. Now you will have `simple-hello-world-example` package pulled from npm, in the node_modules.
3. In the same folder, `node index.js` to see the output.

### Overwriting the same package with a local one:
1. Go to the package1 folder and run `yarn link`.
2. Go back to demo and run `yarn link "simple-hello-world-example"`.
3. Now run `node index.js` to see the different output.

### To go back to the original remote package:
1. Go to the package1 folder and run `yarn unlink`.
2. Go back to demo and run `yarn unlink "simple-hello-world-example"`.
3. Then, you will need to run `yarn install` again.