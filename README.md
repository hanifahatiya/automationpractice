# automationpractice
Webdriver IO Cucumber - Automation Prcatice
This repository contains a collection of test cases webdriverIO-v7 (Selenium - Node.js/JavaScript) projects and libraries using the Cucumber (v7.9.0) BDD framework. It uses the chromedriver NPM package that wraps the ChromeDriver.

# Installation
This project is tested on Node v14.17.1. While earlier versions of node may be compatible, but they have not been verified.

# Config Files
WebdriverIO uses configuration files to setup and execute tests in specific ways. The configuration is fully customizable, and different functions can be invoked before, during and after each test or test suite. Config files can be found in the /test/config/ directory and all end with wdio.conf.js. These can be called via the the cli.

# Run Test
1. Choose a spec on wdio.conf.js, example:
    specs: [
            './tests/features/signin.feature'
        ],
3. Choose a require file on wdio.conf.js, example:
        cucumberOpts: {
          require: [
              './tests/step-definitions/signin/signin.js'
          ],
        }
5. To execute a test specs: npx wdio wdio.conf.js
*Note: Before run test case createaccount.js please change data for field ‘email’ on ./tests/features/createaccount.feature

# Spec Reporters
Test reporter, that prints detailed results to console.
