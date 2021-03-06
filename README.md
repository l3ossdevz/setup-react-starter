# setup-react-starter ![Version](https://img.shields.io/badge/version-1.0.0-green.svg)

React Starter with Create React App + ESLint + Prettier


## Usage

1. Eject React with:

```
yarn eject
```
```
npm run eject
```

Create React App will setup Jest, ESLint and Babel for default configuration.


2. Copy code below to `scripts` section in `package.json` mac

```json
"scripts": {
  "lint": "./node_modules/.bin/eslint {src,test} --color",
  "prettier": "prettier --write '{**/*.{js,jsx,ts,tsx,json,css,scss,md},src/**/*.{js,jsx,ts,tsx,json,css,scss,md},test/**/*.{js,jsx,ts,tsx,json,css,scss,md}}'",
  "prettier:watch": "onchange '{**/*.{js,jsx,ts,tsx,json,css,scss,md},src/**/*.{js,jsx,ts,tsx,json,css,scss,md},test/**/*.{js,jsx,ts,tsx,json,css,scss,md}}' -- prettier --write {{changed}}"
}
```
2. Copy code below to `scripts` section in `package.json` windows

```json
"scripts": {
  "lint": "./node_modules/.bin/eslint {src,test} --color",
  "prettier": "prettier --write {**/*.{js,jsx,ts,tsx,json,css,scss,md},src/**/*.{js,jsx,ts,tsx,json,css,scss,md},test/**/*.{js,jsx,ts,tsx,json,css,scss,md}}",
  "prettier:watch": "onchange {**/*.{js,jsx,ts,tsx,json,css,scss,md},src/**/*.{js,jsx,ts,tsx,json,css,scss,md},test/**/*.{js,jsx,ts,tsx,json,css,scss,md}} -- prettier --write {{changed}}"
}
```

> Use `cross-env` If you use Windows for avoid a problem with path file/folder.

Install dependencies

```
yarn add prettier eslint eslint-config-prettier eslint-config-standard eslint-plugin-import eslint-plugin-node eslint-plugin-prettier eslint-plugin-promise eslint-plugin-standard onchange --dev
```

and remove `eslintConfig` section in `package.json` (Use `.eslintrc` instead.)

3. Copy all files `.eslintrc`, `.editorconfig` and `.prettierrc` to your root folder.

4. Create `test` folder and `**.spec.js` for your test file.

Done!

Happy Coding :heart:
