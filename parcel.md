# Parcel

Bundlers like webpack, gulp are tools that help us compile our sass and css files, concatenate our js files and minify them; but we do have to set up config file for doing it which gets complex on a big project.

Parcel helps here to do the same without configuration

## process

Install

```sh
npm install -g parcel-bundler
yarn global add parcel-bundler
```

Create a package.json file in your project directory using `npm init -y` or `yarn init -y`

Code your files `index.html style.scss script.js ..`

```sh
parcel index.html
```

It will create a dist folder with updated and minfied code for deploying

Open localhost:1234
