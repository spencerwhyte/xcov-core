![logo](http://www.nakiostudio.com/xcov-logo.png)
-------
[![Twitter: @nakiostudio](https://img.shields.io/badge/contact-@nakiostudio-blue.svg?style=flat)](https://twitter.com/nakiostudio)
[![License](https://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://github.com/nakiostudio/xcov/blob/master/LICENSE)

**xcov-core** is a command line tool that parses Xcode `.xccoverage` files.

## Usage

Simply run `xcov-core` supplying the path to your `.xccoverage` file and the path
to the **json** output file that will contain the resulting coverage report.

```
$ xcov-core -s build/EasyPeasy.xccoverage -o report.json -x /Applications/Xcode.app/Contents/Frameworks/IDEFoundation.framework/IDEFoundation
```

### Parameters allowed
* `--source` `-s`: Path to the `.xccoverage` file.
* `--output` `-o`: Path to the resulting `.json` file.
* `--ide-foundation-path` `-x`: Full path to IDEFoundation binary.
* `--version` `-v`: Display version.
* `--help` `-h`: Display this help.

## [xcov](https://github.com/nakiostudio/xcov)
**xcov-core** is the binary that powers [xcov](https://github.com/nakiostudio/xcov),
a Ruby gem that eases the creation of beauty HTML coverage reports and its integration
with CI environments.

## License
This project is licensed under the terms of the MIT license. See the LICENSE file.
