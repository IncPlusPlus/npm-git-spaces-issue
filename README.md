This repo exists to demonstrate an issue with NPM on Windows where the path that NPM will clone a Git repo into has spaces in it. As the path string isn't passed to Git with quotation marks, Git fails with the error "too many commands". Trying the exact same command but wrapping the directory with spaces yields a successful command exit.

## How to replicate
Clone this repo and run `npm install` and watch it fail. As long as your environment is the same as I've described, you should run into the same error as me.