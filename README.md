## TP3 - ST2AWD - Interface Development and Design (I2 - 2425S7)

07-Oct-2024 | SE Promo 2026 | KOCOGLU Lucas


#### Question 1 - Difference between installing a package locally and globally

The difference between installing a package locally and globally is that when you install a package locally, it is installed in the node_modules folder of the current project, while when you install a package globally, it is installed in the global node_modules folder. 
This means that when you install a package locally, it is only available to the current project, while when you install a package globally, it is available to all projects on your machine.

To install globally, we use the `-g` flag. Installing locally doesn't need any flag.

We can install locally package using for specific projects (eg. Vue.js) and install globally package for general use (eg. JSDoc).

#### Exercice 1 - Create a new Vue.js project

To create a new Vue project, we can use the following command:

```bash
vue create vue-oath-microsoft-graph
```

This view is shown in the terminal:

```bash
Vue CLI v5.0.8
? Please pick a preset: 
❯ Default ([Vue 3] babel, eslint) 
  Default ([Vue 2] babel, eslint) 
  Manually select features 
```

After successful installation, the folder `vue-oath-microsoft-graph` with project inside.

#### Question 2 - Webpack and Vue

Webpack bundle all the files in the project into a single file. This is useful because it reduces the number of requests that the browser has to make to the server, which can improve the performance of the application.

#### Question 3: The role of Babel and how browserslist may configure its output?

The role of Babel is to transpile the Js code to a version that is compatible with all browsers.
To configure the output of Babel, we can use the browserslist configuration file (`.browserslistrc`) or in `package.json`.
Here's an example:
```json
  "browserslist": [
    "> 1%",
    "last 2 versions",
    "not dead",
    "not ie 11"
  ]
```

#### Question 4: The role of ESLint

ESLint is a tool that helps to identify and fix problems in the code. It checks the code for errors, style issues, and other problems, and provides suggestions for how to fix them.
Current configuration is as following:

```json
  "eslintConfig": {
    "root": true, // to prevent ESLint from looking for configuration files in parent directories
    "env": {
      "node": true // to enable Node.js global variables
    },
    "extends": [
      "plugin:vue/vue3-essential", // to enable Vue.js specific rules
      "eslint:recommended" // to enable recommended rules
    ],
    "parserOptions": {
      "parser": "@babel/eslint-parser" // to enable Babel parser, which allows ESLint to understand modern JavaScript syntax
    },
    "rules": {} // to enable custom rules, no rules here
  },
```

#### Exercise 2: Run serv

To run server, we can use the following command:

```bash
npm run serve
```

![We can see the default page of Vue.js.](https://raw.githubusercontent.com/LucasKoc/TP3-ST2AWD/refs/heads/main/Ressources/Screenshot%202024-10-04%20at%2010.05.22.png "Default page of Vue.js")

#### Exercise 3: Cleanup the project

After deleting the `HelloWorld.vue` file, and all related assets in the `App.vue` file, we can see the following result:

![We see nothing but the text we placed in our page](https://raw.githubusercontent.com/LucasKoc/TP3-ST2AWD/refs/heads/main/Ressources/Screenshot%202024-10-04%20at%2010.17.59.png "Empty page with a little message saying that there is nothing like in the subject")

#### Exercise 4: Create a new component

To create the HomePage, we create a new file `HomePage.vue` in the `src/pages` folder, and update `App.vue` file. We can see the following content:

![We see our new page with HomePage components](https://raw.githubusercontent.com/LucasKoc/TP3-ST2AWD/refs/heads/main/Ressources/Screenshot%202024-10-04%20at%2010.38.50.png "Our new page with HomePage components")


