## Problem Description

When the tsconfig moduleresolution is set to "nodenext", the @apollo/server can't be imported because: The current file is a CommonJS module whose imports will produce 'require' calls; however, the referenced file is an ECMAScript module and cannot be imported with 'require'.

But, changing the moduleresolution to "node" will make the import work.

## Steps

`npm install`

1. Run the build and see the error

`npm run build`

2. Change the tsconfig.json "moduleResolution" value to "node".
3. Run the build again and it should build

`npm run build`
