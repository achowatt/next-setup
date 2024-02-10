## How I created this project:

```
.nvmrc file should have the current node v "v20.11.0"
```

https://vercel.com/docs/cli

```
yarn global add vercel
# or
npm i vercel --global
```

Link vercel ENV

```
vercel link
```

Check vercel cli env

```
vercel env pull env.local
```

Checkout ntl package

install prettier and add this to dev dependencies

```
  "prettier-plugin-tailwindcss": "^0.4.0",
  "@trivago/prettier-plugin-sort-imports": "^4.0.0",
  "eslint-config-prettier": "^9.1.0",
  "prettier": "^2.0.2"
```

Create prettier.config.cjs in the root (see content in the file)

Create .prettierignore file (See content inside the file)

Add "debug-prettier": "npx prettier --debug-check ." to script in package.json

Add "format-prettier": "prettier --write ." to script in package.json

Create .vscode folder with settings.json file, in the root folder -- this allow you to format prettier on save and override local prettier

Add this to dev dependencies

```
 "@typescript-eslint/eslint-plugin": "^6.20.0",
"@typescript-eslint/parser": "^6.20.0",
"eslint": "^8",
"eslint-config-airbnb-base": "^15.0.0",
"eslint-config-airbnb-typescript": "^17.1.0",
"eslint-config-next": "14.1.0",
"eslint-config-prettier": "^9.1.0",
"eslint-plugin-react": "^7.33.2",
```

Add this to package.json -- scripts

```
"build": "next lint && build",
```
