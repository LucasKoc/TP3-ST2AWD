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

This view is shown in the terminal

```bash
Vue CLI v5.0.8
? Please pick a preset: 
❯ Default ([Vue 3] babel, eslint) 
  Default ([Vue 2] babel, eslint) 
  Manually select features 
```

After successful installation, the folder `vue-oath-microsoft-graph` with project inside.
