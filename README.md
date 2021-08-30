# THIS REPO IS NOW ARCHIVED
This issue has been fixed so there is no longer a need for this repository. I may end up deleting it later down the line if I feel it's no longer necessary to keep around.

# Purpose
This repo exists to demonstrate an issue with NPM on Windows ([npm/cli#2414](https://github.com/npm/cli/issues/2414)) where the path that NPM will clone a Git repo into has spaces in it. As the path string isn't passed to Git with quotation marks, Git fails with the error "too many commands". Trying the exact same command but wrapping the directory with spaces yields a successful command exit.

## How to replicate
Clone this repo and run `npm install` and watch it fail. As long as your environment is the same as I've described, you should run into the same error as me.
