# JS/TS semantic versioning primer script

I built this script to simplify one step of my (and probably someone else's) JS/TS application project initialization processes.

Note: Script makes assumption that you have already initialized the project AND you're running it in the project directory.

Script does for you what you're hopefully going to do anyway: add semantic versioning into your project.

Basicly script utilizes [this guide](https://dev.to/stijnva/semantic-versioning-in-javascript-projects-made-easy-3h63).

Hopefully it's useful to others too.

## Script overview

Script relies on couple of CLI tools:

- printf
- np[mx]
- sed

Script adds these (dev) dependencies to your project:

- standard-version
- commitizen
- @commitlint/{cli,config-conventional}
- husky

Script adds `commitlint.config.js`-file to your project and also modifies `package.json`-file by adding preferences for `husky` and two new scripts `cm` and `release`.
