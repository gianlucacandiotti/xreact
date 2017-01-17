# xReact

This is an Express template I plan to use for my own projects. It's still work in progress but you can check it out. You can also checkout my [xVue](https://github.com/gianlucacandiotti/xvue) template that uses almost the same configuration but supports Vue.js.

## Why did you do this ?

I'm a Front End developer often starting new projects and felt like an Express.js template with decent configuration for React.js was missing. Most tools for scaffolding out there are configured for SPAs and it's not always the use case. So I setted up this project that is kind of a merge between an express generated app and the configuration of the [vue-webpack template](https://github.com/vuejs-templates/webpack) and the [create-react-app](https://github.com/facebookincubator/create-react-app) project for my future use. It has [Dust.js](http://www.dustjs.com/) as its template engine.

## How can I start a project using this ?

1. `git clone https://github.com/gianlucacandiotti/xreact.git PROJECT_NAME`.
2. `cd PROJECT_NAME && yarn` (or `npm install` if that suites you better).
3. `cp .env-example .env`
4. Modify your .env file to have the HOST variable be the same as your project's url (localhost by default).

You are all set to go. Now you may just run the commands below to start developing !

## What's included

These are the tasks included in the template. I'll use most of the descriptions from the [Vuejs Webpack template](https://github.com/vuejs-templates/webpack) and [create-react-app](https://github.com/facebookincubator/create-react-app) projects since the configuration is a merge of those. If you want to know anything else about the tasks, about the folder structure or how to change or extend anything refer to their docs.

- `npm start`: Runs the express app on port 3000.
  - You can change the port in the .env file.
  - It will automatically load routes created on the routes folder, you just have to export an object with a format from each file. Use the once already created as reference.

- `npm run dev`: First-in-class development experience.
  - The page will reload if you make edits.
  - State preserving compilation error overlay
  - Lint-on-save with ESLint
  - Source maps

- `npm run build`: Production ready build.
  - JavaScript minified with [UglifyJS](https://github.com/mishoo/UglifyJS2).
  - HTML minified with [html-minifier](https://github.com/kangax/html-minifier).
  - CSS across all components extracted into a single file and minified with [cssnano](https://github.com/ben-eb/cssnano).
  - All static assets compiled with version hashes for efficient long-term caching, and a production `base.blade.php` is auto-generated with proper URLs to these generated assets.

- `npm run unit`: Uses the same configuration as a [create-react-app](https://github.com/facebookincubator/create-react-app) generated project.
  - Runs the test watcher in an interactive mode.
  - By default, runs tests related to files changes since the last commit.

- `npm run generate-html`: Generates individual .html files for each route the application handles.
  - For the moment you have to manually keep track of your routes.
  - It automatically creates a folder structure that represent all the routes in the application.

## So, anything else ?

Not really. I'd just want to thank you for giving it a try or at least reading through. If you have any feedback it'd be greatly appreciated. I bet a lot of things could be improved and I'm open to discussion, so open an issue, send a pull request or message me to gianluca.prwlr@gmail.com.
