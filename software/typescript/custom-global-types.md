# Creating Your Own Types
- Create a new `.ts` file that is included in the `tsconfig.json` "include" property.
- Declare types without using `export`. If `export` is used, then the file is considered a `module` and you will need to use the `import` statement if you want to use any of your times. If `export` is not used, all of your types will be available to you in all of your components (in Vue.js, for example).
