# Boilerplate Project
> This repository is the base for a dockerized project with frontend in ReactJs and API in ExpressJs. If you will use the information or the code in this repository, please remember adding a star to support me ❤️

## Fastest usage
> You can fork the repository and run the project locally with the command:
```sh
docker-compose up
```

## Guide Step-by-Step

> *Note: If you are going to use git in your project i suggest to you to add a global `.gitignore` file in the root level to ignore node_modules folders and other file you are not interested it.*

### The frontend application
 In this part we will set a react project with Webpack and Babel. What are they? Basically, webpack is a javascript bundler that bundles the static assets into a big file. Babel, instead, is a transcompiler that converts ES6 Javascript code to an older version of Javascript (usually ES5) for compatibility on all browsers.

> I won't describe deeply them in this guide and I strongly reccommend you to checkout their respective official docs to correctly use them in your future development flow.

#### Setup dependencies
In the root level of you project add a new folder called `frontend`. Move in that folder and run from the terminal the following commands.

To create the skeleton of the package.json file use:
```sh
npm init
```
> You can pass the flag `-y` to use the default values in all fields

Now that we have our base file we can install the required React dependencies:
```sh
npm install -P react react-dom
```
> The flag `-P` is the shortcut for the longer one `--save-prod`. It will save the installed packages in the `depedencies` field on the package.json file.
>
> *Note: it is the option used by default by npm and you can omit it if you prefer*

Let's install the development dependencies. I will split them in two command to breack the Babel and the Webpack ones.

Install the Webpack dependencies with the command:
```sh
npm install -D webpack webpack-cli webpack-dev-server html-webpack-plugin
```
> The flag `-D` is the shortcut for the longer one `--save-dev`. It will save the installed packages in the `devDependencies` field on the package.json file.

Install the Babel dependencies with the command:
```sh
npm install -D @babel/core @babel/preset-react @babel/preset-env babel-loader
```
> *Note: if you would like to use `.css` files in your project I suggest to you to install also `style-loader` and `css-loader`.*
