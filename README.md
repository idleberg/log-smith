# log-smith

[![npm](https://img.shields.io/npm/l/log-smith.svg?style=flat-square)](https://www.npmjs.org/package/log-smith)
[![npm](https://img.shields.io/npm/v/log-smith.svg?style=flat-square)](https://www.npmjs.org/package/log-smith)
[![Travis](https://img.shields.io/travis/idleberg/log-smith.svg?style=flat-square)](https://travis-ci.org/idleberg/log-smith)
[![David](https://img.shields.io/david/idleberg/log-smith.svg?style=flat-square)](https://david-dm.org/idleberg/log-smith)
[![David](https://img.shields.io/david/dev/idleberg/log-smith.svg?style=flat-square)](https://david-dm.org/idleberg/log-smith?type=dev)

Creates a Markdown changelog from your GitHub releases

## Installation

`npm install -g log-smith`

## Usage

This is a CLI applicaiton. See `log-smith -h` for a list of all available options.

```sh
# Create a changelog for the node-atomizr repository
$ log-smith -o idleberg -r node-atomizr > CHANGELOG.md
```

GitHub's API has a rate limit, allowing 60 requests per hour. You can extend this by providing an [access token](https://github.com/settings/tokens):

```sh
$ log-smith -o idleberg -r node-atomizr -t <PRIVATE_ACCESS_TOKEN> > CHANGELOG.md
```

When neither providing owner or repository, `log-smith` will try and use a `package.json` in the current working directory.

## License

This work is licensed under [The MIT License](https://opensource.org/licenses/MIT)

## Donate

You are welcome support this project using [Flattr](https://flattr.com/submit/auto?user_id=idleberg&url=https://github.com/idleberg/log-smith) or Bitcoin `17CXJuPsmhuTzFV2k4RKYwpEHVjskJktRd`