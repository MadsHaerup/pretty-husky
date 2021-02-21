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

install a pre-commit hook for prettier, husky and lint-staged
* `npx mrm lint-staged` 
* add "prettier": "prettier --write ." to scripts or use "prettier --write src/" to only format files in the src folder etc.

By running `npm run prettier`, we can now manually prettify the files.

install husky folder
* `npx husky install`

install a pre-commit hook for our tests, 
* `npx husky add .husky/pre-commit "npm test"` 
* add npm run prettier to the pre-commit file

### Install cross-env
`npm i -D cross-env`

in package.json: `"test": "cross-env CI=true react-scripts test"`


## Want a deeper understanding, go to:

[Husky Webpage](https://typicode.github.io/husky/#/)

[Prettier Webpage](https://prettier.io/)
