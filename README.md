## Blue mix starter

## Description
A starter pack for nodejs with bluemix deployment.

## Requirements
* node `^7.2.0` https://nodejs.org/en/
* npm `^3.10.0`

## Configuration

|Name|Description|
|----|-----------|
|`PORT`| The port to listen|
|`VERBOSE_LOGGING`| The flag if debug logging in enabled|


## Local deployment

|`npm run <script>`|Description|
|------------------|-----------|
|`start`|Serves the app in prod mode. It will override config with `config/production.js`|
|`dev`|Same as `npm start`, but enables nodemon for the server as well.|
|`lint`|Lint all `.js` files.|
|`lint:fix`|Lint and fix all `.js` files. [Read more on this](http://eslint.org/docs/user-guide/command-line-interface.html#fix).|
|`spec`|Run unit tests|
|`spec:watch`|Run unit tests in watch mode|
|`e2e`|Run e2e tests|
|`e2e:watch`|Run e2e tests in watch mode|
|`coverage`|Run unit tests and verify coverage|
|`check-coverage`|Verify coverage only|
|`test`|Run lint, tests and checks coverage|


## Bluemix deployment
1. go to https://console.eu-gb.bluemix.net
2. click *Create app*
3. pick *SDK for Node.js*
4. pick any free *App name* and click *Create*
5. Click on the app and go to tab *Getting started*
6. (optional) Copy manifest.yml from *DOWNLOAD STARTER CODE* to the application directory
7. Complete steps 2-7 for deployment
8. if you copied `manifest.yml` you can just run `cf push` for redeployment

## Testing
Import `postman/Bluemix starter.postman_collection.json` collection and `postman/bluemix starter.postman_environment.json` environment.  

Live demo http://sky-bluemix-starter.eu-gb.mybluemix.net/api/test  
