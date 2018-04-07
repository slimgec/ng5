# Ng5

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.7.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## Following youtube video https://www.youtube.com/watch?v=oa9cnWTpqP8 
Learn Angular 5 in less than 60 Minutes - Free Beginner's Course

## First thing we did was start the server using
ng serve
Then navigated to `http://localhost:4200/` to see app

## Generating components.  These commands make new folders in the src/app directory called home & about
ng generate component home
ng g c about
ng generate service data

## To deploy for production
ng build --prod

## If your app does not require a backend server, you can copy the files out of the dist directory
## If you put in a subdirectory, then run the command
ng build --prod --base-href="myurl"

## Can also deploy with gitpages by running
npm install -g angular-cli-ghpages
download git
setup a github repo
create a github account
call it ng5
git add .
git commit -m "first commit"
git remote add origin https://github.com/slimgec/ng5.git
git push -u origin master
ng build --prod --base-href="https://github.com/slimgec/ng5"
angular-cli-ghpages


## Terminology
*.scss is called a sass file
