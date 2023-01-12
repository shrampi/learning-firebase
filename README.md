# Firebase Notes

## Basics
- install firebase dev dependency
- copy config from project page and initialize app in entry point (index.js)

## Hosting
Setup
- install firebase-tools dev dependency for CLI
- you can access CLI with /node_modules/.bin/firebase
- run `login`
- run `init hosting` for setup wizard

Serving Locally
- run `init emulators`
    - this emulates firebase production env on your local machine
- firebase.json is used for server config
    - add page redirects
    - add headers to endpoints, for example enabling cors for a json file

Preview Channels
- preview channels let you preview changes to project in production with a temporary url
    - you can use github actions to deploy a preview for every pull request
- Manually deploy with `hosting:channel:deploy <channel name>`
    - can optionally add `--expires <time>` to manage time up