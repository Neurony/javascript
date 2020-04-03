### eslint-config-neurony

# Setup

### 1. In project root run:
```sh
npm i eslint-config-neurony
```

### 2. In project root make a folder called ‘styleguide’ and in it create a new eslint-config.js file:
```sh
mkdir styleguide
cd styldeguide
touch eslint-config.js
```

### 3. Open eslint-config.js and add the following lines:
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

### 4. Append this line to package.json scripts: (your js path may differ)
```
"eslint": "npx eslint -c styleguide/eslint-config.js resources/assets/js/front/app.js --fix",
```

## 5. For multiple files, the package.json before mentioned line should look like this:

```
"eslint": "npx eslint -c styleguide/eslint-config.js resources/assets/js/front/app.js --fix",
```


# Running

```sh
npm run eslint
```



