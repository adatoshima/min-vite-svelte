
# minimal vite svelte template
  

a minimal svelte development template

  

## how to create
```bash
$ pnpm create vite
# project name: ....
# Select a framework: ›  Svelte
# Select a variant: ›  JavaScript
```
 

## get rid of a11y warnings
modify svelte.config.js:
```js
export default {
  compilerOptions: {
    warningFilter: (warning) => !warning.code.startsWith('a11y')
  }
}
```
see https://github.com/sveltejs/language-tools/issues/650#issuecomment-2260462839
