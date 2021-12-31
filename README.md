# pocket-deduper <!-- omit in toc -->

[![Build Status](https://github.com/kevinpollet/pocket-deduper/workflows/build/badge.svg)](https://github.com/kevinpollet/pocket-deduper/actions)
[![Go Report Card](https://goreportcard.com/badge/github.com/kevinpollet/pocket-deduper)](https://goreportcard.com/report/github.com/kevinpollet/pocket-deduper)
[![License](https://img.shields.io/github/license/kevinpollet/pocket-deduper)](./LICENSE)

Remove duplicates from your [Pocket](https://app.getpocket.com/) list.

## Table of Contents <!-- omit in toc -->

- [Install](#install)
- [Usage](#usage)
- [Authorization](#authorization)
- [Contributing](#contributing)
- [License](#license)

## Install

```shell
go get github.com/kevinpollet/pocket-deduper
```

## Usage

```shell
pocket-deduper [options]

Options:
-consumerKey  Pocket API consumer key.
-dryRun       Print duplicate items without removing them from Pocket.
-help         Prints this text.
```

## Authorization

The **pocket-deduper** CLI must be authorized to access your Pocket account through the [API](https://getpocket.com/developer/).
The first step is to obtain a `Consumer key` used by the CLI to negotiate an access token:   

1. Go to https://getpocket.com/developer/apps/new.
2. Enter the App `name` and `description`.
3. Select `Retrieve` and `Modify` permissions.
4. Select `Desktop` platform.
5. Accept the Terms of Service.
6. Create Application.
7. Copy and keep your `Consumer Key` secret.

Then, you will have to pass this `Consumer Key` as a CLI flag as described in the [Usage](#usage) section.  

## Contributing

Contributions are welcome!

Want to file a bug, request a feature or contribute some code?

1. Check out the [Code of Conduct](./CODE_OF_CONDUCT.md).
2. Check for an existing [issue](https://github.com/kevinpollet/pocket-deduper/issues) corresponding to your bug or feature request.
3. Open an issue to describe your bug or feature request.

## License

[MIT](./LICENSE)
