# VSCode extension bug repro

https://github.com/sveltejs/kit/pull/8679

Clone this repo...

```bash
git clone git@github.com:Rich-Harris/svelte-vscode-prettier-repro
cd svelte-vscode-prettier-repro
code .
```

...and install dependencies:

```bash
cd projects/test-project
npm install
```

Make an innocuous change to one of the `.svelte` files that Prettier will fix.

Run 'Format Document' from the workspace root. Notice that nothing happens. Now run 'Format Document' from inside `projects/test-project`. Notice that Prettier formats the document.
