# Missing node_modules/.bin with hoisted linker

There is an issue with hoisted linker.

With clean node_modules and after first `pnpm install` node_modules/.bin in packages are not created.
So when run `pnpm build` there is an error about missing command.

After running `pnpm install` the second time node_modules/.bin are created and `pnpm build` in packages start to work.
