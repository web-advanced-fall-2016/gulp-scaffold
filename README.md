# Gulp Scaffold

This gulp scaffold is adopted from [Google Web Started Kit](https://developers.google.com/web/tools/starter-kit/) and modified to meet the requirement for our class assignments. It automates the following tasks in your development:

### Features

| Feature                          | Description                              |
| :------------------------------- | :--------------------------------------- |
| **Sass support**                 | Compile [Sass](http://sass-lang.com/) into CSS with ease, bringing support for variables, mixins and more. |
| **Performance optimization**     | Minify and concatenate JavaScript, CSS, HTML and images to help keep your pages lean. |
| **Code Linting**                 | JavaScript code linting is done using [ESLint](http://eslint.org/) - a pluggable linter tool for identifying and reporting on patterns in JavaScript. Web Starter Kit uses ESLint with [eslint-config-google](https://github.com/google/eslint-config-google), which tries to follow the Google JavaScript style guide. |
| **ES2015 via Babel 6.0**         | ES2015 source code will be automatically transpiled to ES5 for wide browser support. ES2015 support is provided using [Babel](https://babeljs.io/). To disable ES2015 support add the line `"only": "gulpfile.babel.js"`, in the [.babelrc](https://github.com/google/web-starter-kit/blob/master/.babelrc) file. |
| **Built-in HTTP Server**         | A built-in server for previewing your site locally while you develop and iterate |
| **Live Browser Reloading**       | Reload the browser in real-time anytime an edit is made without the need for an extension. |
| **Cross-device Synchronization** | Synchronize clicks, scrolls, forms and live-reload across multiple devices as you edit your project. Powered by [BrowserSync](http://browsersync.io/). (Open up the IP provided on other devices on your network) |



### Commands

Following table lists the tasks provided with the scaffold and their commands:

| Command      | Description                              |
| ------------ | ---------------------------------------- |
| `gulp serve` | Creates a local HTTP server, watches all the files for changes, lints javascript, compiles sass files. |
| `gulp clean` | Cleans the temporary and production codes published in `.tmp/` and `dist/` folders. |
| `gulp build` | Builds the production version of the application under `dist/` folder. It lints the code as well as performance optimization for images,HTML,CSS and JS files. |



### How to use

In order to incorporate the scaffold into your assignments, download this repository in `.zip` format. Uncompress it and copy the content to your fresh project folder. Make sure to copy the hidden files as well! If you can't see your hidden files, you will need to copy the files with command line OR run the following the commands to make your hidden files visible:

`defaults write com.apple.finder AppleShowAllFiles YES`

`killall Finder /System/Library/CoreServices/Finder.app`



In case you want to add the scaffold to an already existing project, you will need to merge your project's dependencies listed in your `package.json` to this scaffold's dependencies listed under its `package.json`. 

Before anything, make sure you have `gulp` globally installed on your computer. If you don't, install it globally using the following command:

`sudo npm install -g gulp`

Next, you need to install the dependencies. Do so by running the following command from the root directory of your project ( where you have the `package.json`). Note that it might take few minutes depending on your connection speed.

`npm install`

After getting the dependencies installed, you should be able to run gulp using the commands mentioned in the [Commands Section](#commands).



### SMACKS

With inside the scaffold, under `www/styles/` you can find a file structure for SASS development. It is an scalable and modular architecture for CSS/SASS development. Find more information about it at: [SMACK](https://smacss.com/). This smacks architecture implementation was adopted from Roy Vanegas [repository](https://github.com/code-warrior/gulp-template-for-html-css-sass-js).