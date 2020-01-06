# Token Manager Custom Quasi-transferable feature

[![lerna](https://img.shields.io/badge/maintained%20with-lerna-cc00ff.svg)](https://lerna.js.org/)

## Development notes

### To update the upstream codebase from A1 repo

```sh
# First add the aragon repo remote and fetch it
`git remote add aragon git@github.com:aragon/aragon-apps.git`
`git fetch aragon master`

# Checkout latest master branch, but just the token-manager changes
`git checkout aragon/master apps/token-manager`
```

From that stage, solve any eventual merge conflict and then commit the changes

Remember to take care of keeping whitelist-oracle related code to avoid breaking the feature

## Publishing to npm

- Login with `npm login`
- Ensure tests are passing with `npm test` before trying to publish
- Run `npx lerna publish` and follow the steps
