# Next.js 15 App Router Bug: Missing page.js

This repository demonstrates a bug in Next.js 15's App Router where the application fails to render the page if a file named `page.js` is missing from the directory. The default export function `Home` is ignored causing a blank screen instead of displaying the expected content.

## Steps to reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Observe the blank screen.

## Solution

The solution involves ensuring that a `page.js` file exists in the directory, even if it's empty, to trigger the expected rendering behavior. For proper structure it is recommended to have a layout folder in the `app` directory and to use the default export function in `page.js` to generate the expected result.
