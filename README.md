# vue
This is to create a knowledge base of best practices and tricks for vuejs.

## Vue Installation
1. REQUIREMENTS: npm && node:16 && @vlue/cli
2. RUN: `sudo npm install -g @vue/cli`
3. RUN: `vue create <name-of-project>` (Might need to install `sudo npm install -g n` && run `sudo n stable` to get a working version of node)
4. SELECT: `Manually select features`
5. SELECT ALL: `Babel`, `Typescript`, `Router`, `Linter / Formatter` (`Unit Testing` && `E2E Testing` are optional)
6. SELECT: `3.x`
7. SELECT: `Use class-style component syntax? N`
8. SELECT: `Use Babel alongside TypeScript? Y`
9. SELECT: `Use history mode for router? Y`
10. SELECT: `ESLint + Prettier`
11. SELECT: `Lint on save`
12. SELECT: `Jest` (if selectd unit testing)
13. SELECT: `Cypress` (if selected E2E testing)
14. SELECT: `Where do you prefer placing config for Babel, ESLint, etc.? In dedicatd config files`
15. SELECT: `Save this as a present for future projects? N` (Unless you'd like the option to save it)


## Configuration files

### vue.config.js
* Any `vuejs` specific configuration will be put in this file.

### tsconfig.json
* Any typescript specific configuration will be put in this file.

### package.json
* Package manager (for downloads).
* Simplify the running of scripts.

### package-lock.json
* Keeps track of the exact npm package versions that are downloaded (they are `locked` to specific versions).

### jest.config.js
* Any unit-test configuration will take place in this file.

### cypress.json
* Any E2E testing will take place in this file.

### Babel.config.js
* Configuration to convert ECMAScript 2015+ into a backwards compatible version of JavaScript for current/older browsers or environments.

### .eslintrc.js
* Automatically lets you know if your styling is not the same.
* All enforced styling rules (or plugins with sets of rules) will be found in this file.

### .browerslistrc
* Specifies which browsers are supported.
  * > 1% - Browsers selected by gloabl usage statistics (the browser is used by at least 1% of the people).
  * last 2 versions - Supports the last 2 versions for each browser.
  * not dead - Exclude browsers without official support in the last 24 months.
  * not ie 11 - Exclude Internet Explorer v11.


## Vue Project Files

### assets
* Any resources that are needed with the project (usually use for images).

### components
* Reusabe UI code.

### router
* Maps the url to a view/component.
* Additional options (such as path parameters AND auth guards) can be added to specific routes.

### views
* Non-reusable main website pages.

### main.ts
* Mounts the project to the root element (`<div id="app"></div>` in this case, found in index.html), so that the project has a starting point.
* Multiple vue projects could be mounted to different root elements if wanted (and if not creating a Single-Page Application (SPA)).

### shims-vue.d.ts
* Helps the IDE know what `.vue` file types are (and how webpack should load them?).

### tests
* Contains both unit and E2E tests.
