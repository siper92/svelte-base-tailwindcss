# Svelte Starter Project

### Tech Stack

- Svelte - 3
- Snowpack
- TypeScript
- TailWindCss with PostCSS and SCSS

### Scripts

- run the dev server

```bash
npm run dev
```

- build and test the site

```bash
npm run build
# to start a nginx server to serve the files
docker run --rm --name web -v /$(pwd)/build:/usr/share/nginx/html -p 80:80 nginx
```

### Debugging problems

- for problems with svelte language server make sure the you have the "svelte.language-server.runtime" set to the correct node version

```
"svelte.language-server.runtime": "/home/redder/.nvm/versions/node/v15.3.0/bin/node"
```
