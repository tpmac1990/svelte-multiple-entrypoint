# Demo Svelte App
A simple app to demonstrate svelte

## setup
`npx degit sveltejs/template moz-todo-svelte`
`cd moz-todo-svelte`
`npm install`
`npm run dev`
goto `localhost:8080`
to deploy `npm run build`
`surge public` public is the directory it builds to

### view both entry points
once the dev server is running:
for the index.html entrypoint:
`http://localhost:8080` it will look for `index.html` by default
for the other.html entrypoint:
`http://localhost:8080/other.html`


## setup with webpack instead of rollup
`npx degit sveltejs/template-webpack <name_of_app>`
then use the same commands as above
see `https://github.com/sveltejs/template-webpack`
I have not tried this yet. Rollup seems more than sufficient

### webpack vs rollup
both are good at error handling, but rollup has a slightly smaller build size.
webpack has more plugins.


### errors
UMD and IIFE output formats are not supported for code-splitting builds
Error: Invalid value for option "output.file" - you must set "output.dir" instead of "output.file" when providing named inputs.