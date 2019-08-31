# madbarua.github.io

> A Vue.js project

This project contains a default vue-cli (2.9.6) project using the webpack template. 

- Custom ESLint Rules have been applied.
- Build files from `dist` have been integrated with basic express server
- Has options load page over `http` or `https`



## Local Build Setup

1. `npm install`

2. To load over https, create a `.env` file in the root directory and copy the contents of `.env.example` to it. Set `USE_SSL` to `true|false to load over https before proceeding to #5.

3. `npm run dev` to serve with hot reload at localhost:8080

4. `npm run build` to build for production with minification

5. `npm run dev:server` 
	- serves static build files from express server at localhost:8080
	- if `USE_SSL` is true, https version can be loaded from `https://localhost:8043`


For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).



## Travis CI/CD

The website, accessible from [https://madbarua.github.io](https://madbarua.github.io) uses static build files pushed into the `master` branch.

This can be be manually done by pushing static build files directly into the `master` branch, or automatically by pushing vue project updates into the `dev` branch. Please follow the instructions below for automatic CI/CD using [Travis](https://travis-ci.com/).



### Automactic CI/CD Using Travis

1. Create a branch from `dev`. <br>
`git checkout -b my-test-branch`

2. Create a pull request for branch `dev` from the new `my-test-branch` that you've created.

3. Approve the pull request.

4. View the travis CI status from [https://travis-ci.com/madbarua/madbarua.github.io](https://travis-ci.com/madbarua/madbarua.github.io). (*private account*) <br>
New GitHub pages website updates can be viewed from [https://madbarua.github.io](https://madbarua.github.io) if the build passed.



@madbarua<br>
20190901
