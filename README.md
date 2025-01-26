# Playwright Setup with HTML Report Feature

## Installation

1. Install Playwright:
    ```bash
    npm init playwright/latest
    ```

## Configuration

1. Create a `playwright.config.js` file in the root of your project:
    ```javascript
    // playwright.config.js
    const { defineConfig } = require('@playwright/test');

    module.exports = defineConfig({
      reporter: [
        ['list'],
        ['html', { outputFolder: 'playwright-report' }]
      ],
      use: {
        headless: true,
      },
    });
    ```

## Running Tests

1. Add a test script to your `package.json`:
    ```json
    "scripts": {
      "test": "playwright test"
    }
    ```

2. Run your tests:
    ```bash
    npm test
    ```

## Viewing the Report

After running your tests, the HTML report will be generated in the `playwright-report` folder. Open the `index.html` file in your browser to view the report.

## Learning Resources

Here are some resources to help you learn more about Playwright:

- [Playwright Documentation](https://playwright.dev/docs/intro)
- [Playwright GitHub Repository](https://github.com/microsoft/playwright)
- [Playwright Examples](https://github.com/microsoft/playwright/tree/main/examples)
- [Playwright YouTube Channel](https://www.youtube.com/channel/UC46Zj8pDH5tDosqm1gd7WTg)
- [Playwright Community Discussions](https://github.com/microsoft/playwright/discussions)

These resources provide comprehensive guides, examples, and community support to help you get the most out of Playwright.