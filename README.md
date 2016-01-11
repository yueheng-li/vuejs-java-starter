# vuejs-java-starter

> Vue.js spring boot starter project

## CHANGELOG:

## 0.0.3 (2016-01-11)

* Added basic vue-resource example
* Configured proxy from webpack-dev-server to backend
* Added .editorconfig

## Run in production mode

``` bash
# compile and start in production mode
 mvn spring-boot:run
```

server will start on [http://localhost:8080/](http://localhost:8080/)

## Run in development mode

``` bash
# compile and start in development mode
 mvn spring-boot:run -Dspring.profiles.active=dev

# start webpack development server for HMR
 npm run dev
```

java server will start on [http://localhost:8080/](http://localhost:8080/)
webpack server will start on [http://localhost:3000/](http://localhost:3000/)

Hot module replacement will be available from both servers

##Running tests

``` bash
# run karma tests
 npm run tests
 
# run java and karma
 mvn test
```

## Directory structure

```
.
├ build                   # webpack build configuration
├ .mvn                    # maven wrapper directory
├ node                    # maven will install node here
├ node_modules            # node modules
├ target                  # compiled java sources
├ src                     # sources
│  ├ main                 
│  │  ├ java                           # java sources
│  │  ├ vuejs                          # javascript sources
│  │  └ resources                      # resources
│  │     ├ static                      # static resources
│  │     │   ├ css                          # styles
│  │     │   ├ images                       # images
│  │     │   ├ dist                         # generated javascript goes here
│  │     │   └ index.html                   # development index.html
│  │     └ application.properties      # spring boot configuration properties
│  └ test                       # test sources
│      ├ java                   # java tests
│      └ vuejs                  # vue.js tests
├ .babelrc                 # babel configuration
├ .eslintrc                # eslint configuration
├ .gitignore               # gitignore
├ package.json             # node configuration
├ pom.xml                  # maven configuration 
├ mvnw                     # maven linux wrapper
├ mvnw.cmd                 # maven windows wrapper
├ npm                      # local npm linux wrapper
├ npm.cmd                  # local npm windows wrapper
└ README.md                # this file
```
