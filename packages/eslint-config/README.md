# How to install & use

## 1. In project root run:
```sh
npm i eslint-config-neurony
```

## 2. In project root make a folder called ‘styleguide’ and in it create a new index.js file:
```sh
mkdir styleguide
cd styldeguide
touch index.js
```

## 3. Open index.js and add the following lines:
```js
module.exports = {
  extends: [
    'eslint-config-neurony'
  ].map(require.resolve),
  parserOptions: {
    ecmaVersion: 2018,
    sourceType: 'module',
  },
  rules: {},
};
```

## 4. Append this line to package.json scripts: (your js path may differ)
```
"eslint": "npx eslint -c styleguide/index.js resources/assets/js/front/app.js --fix",
```

## 5. For multiple files, the package.json before mentioned line should look like this:

```
"eslint": "npx eslint -c styleguide/index.js resources/assets/js/front/app.js --fix",
```

To run:
```sh
npm run eslint
```

