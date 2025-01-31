<p align="center">
  <img alt="Nimble logo" src="https://assets.nimblehq.co/logo/light/logo-light-text-320.png" />
</p>

<p align="center">
  <strong>React Template CLI Tool</strong>
</p>

---

<p align="center">
  <a href="https://www.npmjs.com/package/@nimblehq/react-templates"><img src="https://badgen.net/npm/v/@nimblehq/react-templates" /></a>
  <a href="https://www.npmjs.com/package/@nimblehq/react-templates"><img src="https://badgen.net/npm/dy/@nimblehq/react-templates" /></a>
</p>

Command Line Interface for React application at Nimble.

This CLI is built with the [Open CLI framework](https://oclif.io/) [![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g @nimblehq/react-templates
$ nimble-react COMMAND
running command...
$ nimble-react (--version)
@nimblehq/react-templates/0.0.0 darwin-x64 node-v16.14.2
$ nimble-react --help [COMMAND]
USAGE
  $ nimble-react COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`nimble-react generate APP_NAME`](#nimble-react--generate-app_name)
* [`nimble-react help [COMMAND]`](#nimble-react--help-command)

## `nimble-react generate APP_NAME`

Say hello

```bash
USAGE
  $ nimble-react generate [APP_NAME]

FLAGS
  -c, --versionControl=<value> (optional) version control to use in the project (options: github,gitlab,none)

DESCRIPTION
  Generate CRA application

EXAMPLES
  $ nimble-react generate my-app --versionControl github
```

## `nimble-react help [COMMAND]`

Display help for nimble-react.

```bash
USAGE
  $ nimble-react help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for nimble-react .
```
<!-- commandsstop -->

## How to contribute

### Run

To run the CLI on your local machine:

```bash
  $ cd ./packages/cli-tool/
  $ npm i
  $ ./bin/dev generate app-name
```

> 💡 Running just `./bin/dev` without argument will display all the possible commands as well as additional information.

If your changes also impacted the `cra-template` package, you can still test them locally using:

```BASH
  ./bin/dev generate test-cli file:../cra-template
```

Find more the [OCLIF Documentation](https://oclif.io/docs/introduction.html)!

### Test

Tests are generated from the combination of:
- `TestData` objects
- `Scenario` objects

`TestData` objects gather all the rules that should be tested for a given add-on.
When creating a new add-on, you need to create a new associated TestData object in the `./test/add-ons/**` folder.

`Scenario` objects enable running the tests of multiple add-ons in a single `generate` command execution. As running the `generate` command is time-consuming, grouping several add-ons tests into a single scenario is a way to get tests results earlier.

## License

This project is Copyright (c) 2014 and onwards.
It is free software and may be redistributed under the terms specified in the [LICENSE] file.

[LICENSE]: /LICENSE

## About

![Nimble](https://assets.nimblehq.co/logo/dark/logo-dark-text-160.png)

This project is maintained and funded by [Nimble](https://nimblehq.co).

We love open source and do our part in sharing our work with the community!
See [our other projects][community] or [hire our team][hire] to help build your product.

[community]: https://github.com/nimblehq
[hire]: https://nimblehq.co/
