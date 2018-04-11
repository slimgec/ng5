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

## Start of Project - ng5
This project was developed using the Learn Angular 5 in less than 60 Minutes - Free Beginner's Course by Gary Simon
(youtube video https://www.youtube.com/watch?v=oa9cnWTpqP8).
A written version of this video can be found at coursetro.com (https://coursetro.com/courses/19/Learn-Angular-5-from-Scratch---Angular-5-Tutorial)

## Installing prerequisites
Install node and npm (https://nodejs.org/en/download/)  
node -v  
npm -v

Install angular (sudo npm install @angular/cli -g)  
ng -v

## Creating a new project
cd src  
ng new ng5 --style=scss --routing

## Starting the local server
cd ng5 
ng serve
Then navigated to `http://localhost:4200/` to see app

## Generating components.
The following commands make new folders in the src/app directory called home & about:  
g is short for generate, c is short for component, s is short for service   
ng generate component home  
ng g c about  
ng generate service data  

## To deploy for production
ng build --prod

## Simple Deploy
If your app does not require a backend server, you can copy the files out 
of the dist directory. If you put in a subdirectory, then run the command

ng build --prod --base-href="myurl"

## Deploy using gitpages
npm install -g angular-cli-ghpages  
download git  
setup a github repo  
create a github account  
call it ng5  
git add .  
git commit -m "first commit"  
git remote add origin https://github.com/slimgec/ng5.git  
git push -u origin master  
ng build --prod --base-href="https://slimgec.github.io/ng5"  
angular-cli-ghpages  

## Correcting error produced by angular-cli-ghpages command on Mac
I needed to change the directory permissions to make it work.  
angular-cli-ghpages --no-silent  <-- This command shows error messages  
sudo chown -R <myusername> /usr/local/lib/node_modules/angular-cli-ghpages/node_modules/gh-pages/  
Note: it takes a few minutes for github to publish after successful upload

## I did the following, but I don't think it mattered
Copy your public key and go to your GitHub account -> settings -> create a SSH and GPG keys then click new ssh key and past your public key in the in key text field.  

Verify your public key using Git Bash by running the following command:  
ssh -vT git@github.com  
You will get output like this  

    debug1: channel 0: free: client-session, nchannels 1
    Transferred: sent 3848, received 2040 bytes, in 0.2 seconds
    Bytes per second: sent 16032.4, received 8499.5
    debug1: Exit status 1
    
## Note
When you download the source from github, remember to run npm install

## Terminology
A .scss file extension is called a "sassy css" file. (http://www.thesassway.com/editorial/sass-vs-scss-which-syntax-is-better)

A .ts file extension is a type script file. (https://www.typescriptlang.org/)

A .md file extension is a markdown file. (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
