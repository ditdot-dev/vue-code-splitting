# Code Splitting in Vue 
> Code splitting example app that demonstrates creating multiple code bundles with dynamic import statements. 

Example of code splitting in Vue based on computed property and dynamic components. The initial load contains the initial view and critical assets, while other modules are loaded on the button press. 

## Features 

- when the data changes, the computed property will re-evaluate
- dynamic component switches between the imported components after the computed property change
- default Vue CLI prefetch function is disabled in vue.config.js - components are loaded on demand, as the user navigates the application

## Article

- [Code Splitting in Vue](https://www.ditdot.hr/en/code-splitting-in-vue-js)


## Clone

Clone this repo to your local machine 

```shell
$ git clone https://github.com/ditdot-dev/vue-code-splitting-example.git
```

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## License

[MIT](https://github.com/ditdot-dev/vue-code-splitting-example/blob/main/LICENSE) license.
