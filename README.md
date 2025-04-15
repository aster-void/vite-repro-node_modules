# How it works

- bun reads "workspaces" field at root package.json
- bun automatically links all packages whose _path_ match one in "workspaces" to root package
- `bun install` will create node_modules only at root, and every packages required by the workspace packages will be installed to root node_modules

