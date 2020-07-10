# Oxford-Brookes-University-P00412--Big-Data-and-The-Cloud-A-School-Operation-and-Manangement-system (ASOAMS)

ASOAMS Client:                                     

Project setup:

Install dependencies - yarn install

Compiles and hot-reloads for development - yarn serve

Compiles source code for production use - yarn build

Run the server - yarn start

Run the tests - yarn test

Lint and fix files accordingly - yarn lint

Run your end-to-end tests - yarn test:e2e

Run the unit tests - `yarn test:unit

Functionality & Design: 

1.Front-end framework of choice: Vue.js, Bootstrap 4 and Bootstrap-Vue

Vue files: 

How each Vue file works is as follows:


<template></template> - This block syntax allows us to write HTML code along side JavaScript variables that we will push from the <script> block.

<script></script> - This is where we render components, computations, functions into the page right before it is loaded into the DOM. Typicall you will see in each .vue file that we will import modules, libraries and components before executing any other tasks.

<style></style> - This allows us to write scoped styles within the view so it does not affect other pages outside of this scope.


Libraries used: 

We used a mixture of 3rd party libraries and modules to perform tedious actions such as HTTP requests, formatting date and time, creating slugs, formatting names and many more:

Bootstrap 4 framework - Front-end UI framework
FortAwesome FontAwesome - Font icon library
Vue-Axios - To perform HTTP requests to APIs
VueX - State Management for Vue.js to store user data securely
Vue routing - To route different view pages into the DOM


Design architecture: 

The system is built using a combination of Model-View-Controller with modular approach. The code is separated into several folders/categories:


public - Main folder that renders the HTML page in the browser with the latest web standards

src - The root folder where Vue framework is compiled



assets - Contains image assets and css files

components - Contains components that is rendered into DOM such as footer, header, navigation, searchbar, loading screen etc

layouts - Dashboard layout

styles - SCSS files separated into modules for each page that is using it. Again following DRY concept.

views - Pages which are rendered based on the links the user interacts with such as Homepage, Dashboard, Settings, Login, Registration and many more.

App.vue - Renders all of the components, routes and views

main.ts - Initiates the process of compiling the framework

registerServiceWorker.ts - Enables you to setup PWA

router.ts - Routing module that renders the pages

store.ts - State management module using VueX



.nvmrc,.gitignore,.eslintrc.js,vue.config.js,package.json - Configuration files to tailor the application to function ,test and render to our specification

app.yaml - To instantiate a client instance in the cloud


Customize configuration
See Configuration Reference.

Application is based on this tutorial (up-to-date without the complete example with post):
https://appdividend.com/2018/11/21/mevn-stack-tutorial-with-example-from-scratch/

Solve MongoDB Deprecations:
https://mongoosejs.com/docs/deprecations.html

MongoDB URI Connection options are:
https://docs.mongodb.com/manual/reference/connection-string/
