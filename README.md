# Sauce Labs performance demo app

With: 

- Angular 5 + Angular CLI 
- Angular Material 
- ng-Apimock
- protractor-image-comparison

## Intro

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.7.3. 

![App overview](./assets/app-movie.gif "App overview")

## Usage

### Preparation

- `git clone https://github.com/wswebcreation/sauce-perf-demo-app.git`
- `cd sauce-perf-demo-app` to go into the demo folder
- `npm i` - Installs everything needed
- `npm start` - Starts the app.
- `npm run start.mocking` - Starts the mocking.
- go to `http://localhost:4300/` to open the demo app
- go to `http://localhost:3000/mocking/` to open the mocking interface

> **If you get an error like `Error: listen EADDRINUSE :::3000` or `Error: listen EADDRINUSE :::4300` then the port(s)is in use. Please kill the process on that port and try again (Google may be so friendly to help you with that ;-))**

> **Windows: use precompilation to speed up**

    `tsc --project tsconfig.json`
    `npm start`

### Testing with protractor
For running the protractor tests a selenium server needs to be started. The server will automatically be downloaded and updated after install.

To run the tests the the following needs to be started:
- the app, see `npm start` (if not already started)
- the mocking server, see `npm run start.mocking` (if not already started)
- the selenium server. Run `npm run webdriver.start`. If you get an error run `npm run webdriver.update` and try `npm run webdriver.start` again.
- and run the tests, use `npm run e2e`, see [protractor.conf.js](./e2e/config/protractor.conf.js) how to provide specific features / tags

## License

MIT

## Credits
I used this project ([angular5-example-app](https://github.com/Ismaestro/angular5-example-app), made by [Ismael Ramos](https://github.com/Ismaestro)) as an idea and rewritten and adjusted it to our needs.
