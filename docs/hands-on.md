## Forking the Repository

    Fork the original repository: https://github.com/ComunidadeTechQA/qatw-primeira-edicao

## After cloning it in your local machine, enter in the directory and create a new Playwright project

    npm init playwright@latest

![alt text](image.png)

## Run the initial tests (by default they run in three different browsers - Chrome, Firefox and Safari)

    npx playwright test

![alt text](image-1.png)

## By default, playwright projects run in headless mode, to run it in the browser you can try the command below: 

    npx playwright test --headed

## Showing the native report on the browser

    npx playwright show-report

![alt text](image-3.png)
![alt text](image-2.png)

## Manually testing the login

- Having you mailtrap account created, access your inbox at `https://mailtrap.io/inboxes` and get your inbox id to be used in this project and update the values below in the `playwright.config.js` file:
    MAILTRAP_ACCOUNT_ID
    MAILTRAP_INBOX_ID

![alt text](image-4.png)

- Also get you API token and update it in the `MAILTRAP_TOKEN` value in the `playwright.config.js` file:

![alt text](image-5.png)

## Access postgresql database (credentials can be found in the 'docker-compose.yml' file)

    http://paybank-dbadm:15432

a) General tab
![alt text](image-6.png)

b) Connection tab
![alt text](image-7.png)

## Creating login test case using Playwright Codegen

    npx playwright codegen http://paybank-mf-auth:3000

## In order to open the Playwright Test console (similar to what we have with Cypress dashboard), you can use:

    npx playwright test --headed

## To Debug, go with:

    npx playwright test --debug

## 