# JS Neurony Style Guide

### Package name: eslint-config-neurony

### Setup

### In project root run:
```sh
npm i -g eslint
npm i eslint-plugin-import eslint-config-neurony --save-dev 
```

### In your project root create a file called .eslintrc and paste this into it:
    
```sh
{   
  "extends": "eslint-config-neurony",
  "parserOptions": {
    "ecmaVersion": 6
  }
}
```
In this file you can specify any extra rules or settings for your project’s needs.

### Append this line to package.json scripts: (your js path may differ)
```
"eslint": "eslint resources/assets/js/front/*.js --fix",
```


# Running

```sh
npm run eslint
```


# Documentation
