# Corgi Converter
A 2 hour hack to create an Alexa skill for free swag. It's basically a "hello world" application.
The code sucks, feel free to make it better and open PRs. You have been warned.

## Installing
- `git clone https://github.com/ehotinger/alexa-corgi-converter`
- Follow the instructions to set up the [alexa-sdk](https://github.com/alexa/alexa-skills-kit-sdk-for-nodejs).
    - (`npm install --save alexa-sdk`)
- When you build your model, you can use `intents.json` as a reference. `{input}` is set up to be an animal as recognized by Alexa's natural language processing.
- Put your Alexa skill's application id in `index.js`.
- When you publish your AWS Lambda function, upload a `.zip` with the `node_modules` dependencies generated in this step alongside `index.js` at the root.
    - Your Lambda function also needs to take the Alexa Skills Kit as an input.

## Testing
I'd recommend testing two ways:
- For fast iterations, just use Amazon's online Alexa tool to test your Lambda function and various input combinations.
- Once the skill is passing the online test, set up a developer beta and connect your own devices and try it out before publishing.

You can also test locally if you spend more time tinkering with the SDK, but I didn't bother. ;)