# Testing [lightweight to-do list webapp](https://todomvc.com/examples/angular2/) using Cypress

## __Prerequisites__
1. Install [NodeJS](https://nodejs.org)
2. Install [Cypress](https://docs.cypress.io/guides/getting-started/installing-cypress.html#Install-binary)
3. Have Chrome installed

## [Test Plan](testplan.txt)

## __Installing Dependencies__
1. Install Cybress
````
npm install cypress
````
2. To open the Cypress Application use the command
````
npx cypress open
````

3. To run Cypress Headless use the command
````
npx cypress run
````

### 🐛 Bonus bug!
#### Steps to reproduce: 
1. Add a todo.
2. Double-click on it to open edit mode.
3. Delete the text in edit todo field.
4. Unfocus the field without saving changes.
> This todo is neither deleted, nor in edit mode, and its layout is broken.
5. Click on that todo once again.
6. Try to unfocus or delete.
> This todo is back to edit mode but it can't be reverted back, even by adding a new todo.

![alt text](https://media.giphy.com/media/t8sCmiDgr6DUYS56sZ/giphy.gif)

