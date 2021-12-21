## Semestrálka

Vaším úkolem bude zkombinovat látku z kurzu a s využitím GitHub Actions, Docker a Ansible sestavit pipeline.

Pipeline bude rozdělena na dvě větve. Pokud otevřu pull request z nějaké branche do masteru, sestaví se mi eshop, otestuje a povolí mi mergnout kód do masteru. Pokud neprojde, bude merge blokován. V okamžiku merge do masteru se spustí workflow, které kromě kroků z předchozího scénáře ještě nasadí eshop pomocí Ansible na EC2. Po doběhnutí GHA workflow z masteru se vám tedy pokaždé vytvoří nová instance EC2, zůstane vám tam ale i ta stará. Poslední částí toho úkolu je automatické mazání té staré instance. To zajistíte jako další krok ve vašem Ansible playbooku.

## Installation Guide
- Install GIT - https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
- Install Docker - https://www.docker.com/products/docker-desktop

## Build/Run
- Source code of the React app is based on "react-shopping-cart" app made under MIT license by Jefferson Ribeiro

#### Requirements

- Node.js
- NPM

```javascript

/* First, Install the needed packages */
npm install

/* Then start both Node and React */
npm start

/* To run the tests */
npm run test

/* Build sources */
npm run build

/* Running e2e tests */
npm run wdio

/* Deploy to Firebase */
./node_modules/.bin/firebase deploy --token=$FIREBASE_DEPLOY_TOKEN


```

## About tests .

- Unit tests
  - All components have at least a basic smoke test
- Integration tests
  - Fetch product and add to cart properly
- e2e
  - Webdriverio - Add and remove product from cart

### Copyright and license

The MIT License (MIT). Please see License File for more information.

Try to trigger
