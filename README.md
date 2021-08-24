# References for explanation on why the setup has to be done this way

* https://blog.logrocket.com/publishing-node-modules-typescript-es-modules/



* To compile , run the command below

```bash
npm run tsc
```

* this requires `typescript` and `tsc`


# Publishing locally

* see here
https://medium.com/@debshish.pal/publish-a-npm-package-locally-for-testing-9a00015eb9fd
* https://stackoverflow.com/questions/8088795/installing-a-local-module-using-npm
* https://stackoverflow.com/questions/17509669/how-to-install-an-npm-package-from-github-directly


# Adding the subpackage to a main package without building beforehand

* as pointed out [here](https://stackoverflow.com/a/48392815/10045897), the best way to build the package on installation is by specifying the `prepare` step in the `package.json`
* To verify that this works, install by specifying git url directly

* See also [here](https://docs.npmjs.com/cli/v7/configuring-npm/package-json#local-paths)

```bash
# Use abspath explicitly
npm install git+file:/XXX/github_projects/typescript_sandbox_subpackage#master
```

