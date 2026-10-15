## Cypress test template

<!-- This is an Apify template readme -->

Run your [Cypress tests](https://www.cypress.io/) on the Apify Platform effectively and easily. The template provides the necessary setup for running the Cypress tests. You can change the Cypress configuration in the input, which is defined by the [input schema](https://docs.apify.com/platform/actors/development/input-schema). The template uses [globby library](https://www.jsdocs.io/package/globby) to fetch the Cypress test files and run them within the Actor. The video recordings are stored in [Key-value store](https://docs.apify.com/platform/storage/key-value-store) and the comprehensive test results are stored in the [Dataset](https://docs.apify.com/platform/storage/dataset).

## Included features

- **[Apify SDK](https://docs.apify.com/sdk/js/)** - toolkit for building [Actors](https://apify.com/actors)
- **[Input schema](https://docs.apify.com/platform/actors/development/input-schema)** - define and easily validate a schema for your Actor's input
- **[Dataset](https://docs.apify.com/sdk/js/docs/guides/result-storage#dataset)** - store structured data where each object stored has the same attributes
- **[Cypress](https://www.cypress.io/)** - JavaScript Component and E2E testing library

## How it works

You can easily run your tests on the Apify Platform, just copy-paste your test files into `cypress/e2e` folder. The tests' names need to end with `-spec.cy.js`.

You can also customize the test run by specifying other options in the input, e.g. the screen size, video recording, or the default command timeout.

After running the tests, the Apify platform stores the results in a comprehensive way - datasets for JSON results, and key-value store for videos. You can view the results directly on the platform or download them to your local machine using a REST API.

## Resources on Cypress test

- [Cypress test runner](https://apify.com/valek.josef/cypress-test-runner) Actor
- [How to deploy tests to the Apify platform](https://blog.apify.com/deploy-cypress-tests-cloud)
- [Video guide on getting data using Apify API](https://www.youtube.com/watch?v=ViYYDHSBAKM)
- [Integration with Zapier](https://apify.com/integrations), Make, Google Drive and others
- [Video guide on getting data using Apify API](https://www.youtube.com/watch?v=ViYYDHSBAKM)
- A short guide on how to create Actors using code templates:

[web scraper template](https://www.youtube.com/watch?v=u-i-Korzf8w)


## Getting started

For complete information [see this article](https://docs.apify.com/platform/actors/development#build-actor-at-apify-console). In short, you will:

1. Build the Actor
2. Run the Actor

## Pull the Actor for local development

If you would like to develop locally, you can pull the existing Actor from Apify console using Apify CLI:

1. Install `apify-cli`

    **Using Homebrew**

    ```bash
    brew install apify-cli
    ```

    **Using NPM**

    ```bash
    npm -g install apify-cli
    ```

2. Pull the Actor by its unique `<ActorId>`, which is one of the following:
    - unique name of the Actor to pull (e.g. "apify/hello-world")
    - or ID of the Actor to pull (e.g. "E2jjCZBezvAZnX8Rb")

    You can find both by clicking on the Actor title at the top of the page, which will open a modal containing both Actor unique name and Actor ID.

    This command will copy the Actor into the current directory on your local machine.

    ```bash
    apify pull <ActorId>
    ```

## Documentation reference

To learn more about Apify and Actors, take a look at the following resources:

- [Apify SDK for JavaScript documentation](https://docs.apify.com/sdk/js)
- [Apify SDK for Python documentation](https://docs.apify.com/sdk/python)
- [Apify Platform documentation](https://docs.apify.com/platform)
- [Join our developer community on Discord](https://discord.com/invite/jyEM2PRvMU)
