# create-vite 9.3.2 Reproduction

## Steps

1. Use Windows with Node.js v26.4.0 and npm 11.17.0.
2. Run:

   npm create vite@9.3.2 my-app -- --template react

3. Observe ENOENT: template-react missing.

## Package verification

npm pack create-vite@9.3.2 --dry-run

The published tarball contains only five files,
with no template-react directory.

## Workaround

npm create vite@9.3.1 my-app -- --template react
