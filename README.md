# `@nrwl/rspack` generator issue

## Steps I followed

1. generate workspace

```
npx create-nx-workspace@latest my-workspace
```

2. add `@nrwl/rspack` to `package.json`

```
yarn add -D @nrwl/rspack
```

3. try to generate `@nrwl/rspack` app

```
npx nx g @nrwl/rspack:app my-app
```

## Error

```
npx nx g @nrwl/rspack:application my-app

>  NX  Generating @nrwl/rspack:application

✔ Which stylesheet format would you like to use? · css

 >  NX   Cannot find module 'typescript'

   Require stack:
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/@phenomnomnominal/tsquery/dist/src/ast.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/@phenomnomnominal/tsquery/dist/src/index.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/@nrwl/rspack/src/utils/generator-utils.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/@nrwl/rspack/src/generators/configuration/configuration.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/@nrwl/rspack/src/generators/application/application.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/nx/src/config/workspaces.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/nx/src/config/configuration.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/nx/src/command-line/generate.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/nx/src/command-line/nx-commands.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/nx/bin/init-local.js
   - /Users/katerina/Projects/nrwl/test_nx_workspaces/myworkspace/node_modules/nx/bin/nx.js
   Pass --verbose to see the stacktrace.

```
