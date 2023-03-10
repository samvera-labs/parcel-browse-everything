# BrowseEverything (in [Parcel](https://parceljs.org/))

![npm](https://img.shields.io/npm/0.0.1/browse-everything)
[![Build Status](https://circleci.com/gh/jrgriffiniii/parcel-browse-everything.svg?style=svg)](https://circleci.com/gh/jrgriffiniii/parcel-browse-everything)
[![Contribution Guidelines](https://img.shields.io/badge/contributing-guidelines-blue.svg)](./CONTRIBUTING.md)
[![Apache 2.0 License](https://img.shields.io/badge/apache2-license-blue.svg)](./LICENSE)

## Community Support

[![Samvera Community Slack](https://img.shields.io/badge/samvera-slack-blueviolet)](http://slack.samvera.org/)

# Overview

BrowseEverything is a JavaScript file upload library intended for integration into Ruby on Rails applications implemented using the Samvera digital repository framework.

## Product Owner & Maintenance

### Product Owner

[jrgriffiniii](http://github.com/jrgriffiniii)

# Help

The Samvera Community is here to help. Please see our [support guide](./SUPPORT.md).

See the [Samvera Confluence](https://samvera.atlassian.net/wiki/spaces/samvera/overview) for information at the architectural level.

Additionally, new adopters and potential adopters may find the pages here useful: <https://samvera.org/>

Further questions? [Get in touch](https://samvera.atlassian.net/wiki/spaces/samvera/pages/405211682/Getting+Started+in+the+Samvera+Community)

## Development

### Building the Package

```bash
$ yarn build
```

### Viewing and Debugging the Package in the Browser

```bash
$ yarn parcel
```

### Linting the Code Base (using ESLint)

```bash
$ yarn lint
```

### Formatting the Code Base (using Prettier)

```bash
$ yarn format
```

### Executing the Test Suites (using Jest)

```bash
$ yarn test
```

The JavaScript package should now be built within the directory `dist/main.js`.

## License

BrowseEverything is available under [the Apache 2.0 license](LICENSE).

## Publishing

### Testing Locally Using [verdaccio](https://verdaccio.org/)

Using `npm`:

```bash
$ npx verdaccio
$ npm login --scope my-company --registry http://localhost:4873/
# Then, within another terminal
$ npm set registry http://localhost:4873/ --location project
# Please ensure that the "version" property in package.json has been incremented to the next release version
$ npm publish
```

Using `yarn`:

```bash
$ yarn verdaccio
$ npm login --scope my-company --registry http://localhost:4873/
# Then, within another terminal
$ yarn publish --registry http://localhost:4873/ --patch
```

### Publishing Releases to [npm](https://www.npmjs.com/)

Using `npm`:

```bash
$ npm login
# Please ensure that the "version" property in package.json has been incremented to the next release version
$ npm publish
```

Using `yarn`:

```bash
$ yarn login
$ yarn publish --patch
```

## Contributing

If you're working on a PR for this project, create a feature branch off of `main`.

This repository follows the [Samvera Community Code of Conduct](https://samvera.atlassian.net/wiki/spaces/samvera/pages/405212316/Code+of+Conduct) and [language recommendations](https://github.com/samvera/maintenance/blob/main/templates/CONTRIBUTING.md#language). Please **_do not_** create a branch called `master` for this repository or as part of your pull request; the branch will either need to be removed or renamed before it can be considered for inclusion in the code base and history of this repository.

## Acknowledgments

This software has been developed by and is brought to you by the Samvera community. Learn more at the [Samvera Community website](https://samvera.org/).

![Samvera Logo](https://samvera.atlassian.net/wiki/download/attachments/1918631965/samvera-fall-TM-220w.png?api=v2)
