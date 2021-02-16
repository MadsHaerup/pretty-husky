# pretty-husky

## what is it?
It will format your code and run the tests before committing.

The idea of pretty-husky is to automate the time consuming process of manually setting up the following files and commands.


# This is the manually way of doing it
 
### Prettier
 commands for code formatting packages
* `npm i -D prettier`
* `npm i -D eslint-config-prettier`

Files needed to be created 
* .prettierignore
* .prettierrc.json filer

### Pre-commit hook

* Running a command before comitting

#### Pre-commit hooks is used for

* Running prettier
* Running tests

installs a pre-commit hook for prettier
* `npx mrm lint-staged` 

installs husky folder
* `npx husky install`
* add npm test to pre-commit file

installs a pre-commit hook for our tests
* `npx husky add .husky/pre-commit "npm test"` 

### Install cross-env
`npm i -D cross-env`

in package.json: `"test": "cross-env CI=true react-scripts test"`


## Want a deeper understanding, go to:

[Husky Webpage](https://typicode.github.io/husky/#/)

[Prettier Webpage](https://prettier.io/)
