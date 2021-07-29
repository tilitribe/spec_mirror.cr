# spec_mirror

A small test helper which will run the mirroring spec whenever a source file 
is saved. It requires a file watcher like [Guardian.cr](https://github.com/f/guardian) for example.

[![Build Status](https://travis-ci.org/tilitribe/spec_mirror.cr.svg?branch=master)](https://travis-ci.org/tilitribe/spec_mirror.cr)
[![GitHub version](https://badge.fury.io/gh/tilitribe%2Fspec_mirror.cr.svg)](https://badge.fury.io/gh/tilitribe%2Fspec_mirror.cr)

## Installation

Add the development dependency to your `shard.yml`:

```yaml
development_dependencies:
  spec_mirror:
    github: tilitribe/spec_mirror.cr
```

Run `shards install`

## Usage

If you are using [Guardian.cr](https://github.com/f/guardian), add the following
lines to the guardian.yml config file:

```yaml
files: ./src/**/*.cr
run: bin/spec_mirror %file%
```

Then start `guardian` and watch your specs run whenever you save a file in your
`src` dir.

## Contributing

1. Fork it (<https://github.com/tilitribe/spec_mirror/fork>)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Contributors

- [wout](https://github.com/wout) - creator and maintainer
- [tilitribe](https://github.com/tilitribe) - owner and maintainer
