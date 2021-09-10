# PNC Web UI React End-to-End Tests

## Changelog

[Changelog](https://github.com/project-ncl/pnc-web-ui-react-e2e-tests/wiki/Change-logs)

## Prerequisites

1. `Node.js` version >= 14
2. `NPM` version >= 7
3. `Prettier`

## Environment setup

Update the environment `env.json` file with the URL of PNC UI that you want to test at here: ./cypress/fixtures/env.json

```
{
  "PNC_UI_URL": "<URL of PNC UI to Test>"
}
```

NOTE: Headless should be false for CI environments. Set to true when developing / debugging.

## Installation

Prepare project locally:

```bash
git clone <yourGitForkUrl> pnc-web-ui-react-e2e-tests
cd ./pnc-web-ui-react-e2e-tests/
npm install
```

## Running the tests

### GUI

Start your test by following steps:

**1) Deploy the PNC Web UI React to the http://localhost:3000/ (if you are using the default `env.json`)**

**2a) Run the test with Cypress GUI**

```bash
npm run test-gui  # Opens Cypress in the interactive GUI.
```

**2b) Run all tests with command line**

```bash
npm run test-cli   # Run all test cases.
```

**2c) Run specific test with command line**

```bash
npm run test-cli --spec "cypress/integration/<Test Name>.js"  # Run specific test case.
```

**3) Enjoy it!**
