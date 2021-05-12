# nuxt-js
Basics of Nuxt.js

## About
- Vue Framework

### Prerequisites
#### npm and Node.js
- Install:
  - Ubuntu: `sudo apt install nodejs npm`
  - macOS: Download [here](https://nodejs.org)
- Update:
  - Ubuntu: `npm cache clean -f; npm install -g n; n latest`

#### Vue.js
- Install:
  - Ubuntu: `npm install vue`

### Running Nuxt.js
#### Create new app
- `npm init nuxt-app <project-name>`


![Terminal output from `create-new-app`](from-npm.png)


#### Install Nuxt
- After creating the folder and `package.json` file, run: `npm install nuxt`

#### Run existing app
- Navigate to root directory of app
- Run: `npm run dev`

### File Structure
#### From Scratch
- In root directory:
  - `package.json`
    - name, dependencies, scripts
  
  - `yarn.lock` or `package-lock.json` created by installation of Nuxt

  - `nuxt.config.js`
    - add modules, override defaults

  - `pages` directory
    - `index.vue` - default home page
      - `<template>`

  - `components` directory
    - holds all `.vue` components, which are auto imported by nuxt

  - `assets` directory
    - holds uncompiled assets

  - `static` directory
    - holds files that have static names and is directly mapped to root

#### Pages
- `.vue` files automatically routed by nuxt using vue-router configuration
- Navigation to site pages: use `<NuxtLink to="/relative-page">` tags
