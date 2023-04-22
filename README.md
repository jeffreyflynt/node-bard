# Using Google Bard's API w/Node

Medium Article: https://jeffreyflynt02.medium.com/using-google-bards-api-w-node-421c100a63d2

## Dependencies

- Node v18
- node-fetch
- dotenv

## Running

Run `npm install`

### Credentials

Create a `.env` file in the root directory and add `Secure1PSID` & `AT_KEY`.

Go to: https://bard.google.com and open DevTools, Go to Application → Cookies → `__Secure-1PSID` and copy that value and use it for the `Secure1PSID` env variable.

For the `AT_KEY` variable, go to Network → Select XHR → make a sample request in the browser (while devtools is open), click on the request and then click the request and click the Payload tab, and copy that value to `AT_KEY`. In my testing, this value stays the same.

### Prompt

Replace the `""` with your prompt at the top in `main.js` in the `PROMPT` variable.

In the command line, enter: `node main.js`
