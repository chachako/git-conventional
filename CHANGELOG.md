# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

<!-- next-header -->
## [Unreleased] - ReleaseDate

### Fixes

- Relaxed some lifetimes, associating them with the message, rather than `Commit`.

## [0.10.2] - 2021-09-06

### Fixes

- Support scopes with numbers in them, like `x86`

## [0.10.1] - 2021-09-03

### Fixes

- Allow trailing newlines when there is no body

## [0.10.0] - 2021-08-18

### Features

- `Commit::breaking_description` to handle the two potential sources for you

### Breaking Changes

- Moved `<TYPE>` consts to `Type::<TYPE>`.

## [0.9.2] - 2021-05-24

### Features

- `serde` feature for serializing `Commit`.

## [0.9.1] - 2021-01-30

## [0.9.0] - 2020-05-06

### Breaking Changes

- Made error type work as `Send` / `Sync`.

## [0.8.0] - 2020-05-06

### Breaking Changes

- `::new` has been renamed to `::new_unchecked` to signify that it bypasses validity checks.

## [0.7.0] - 2020-05-05

### Breaking Changes

- Forked `conventional` as `git-conventional`
- Merged `Simple` and `Typed` APIs (identifiers are typed, otherwise `str`s), removing the need to pull in a trait.

### Features

- Add typed identifier equality with `str`.
- Added constants for common `type_`s.
- Made it easier to find the footer that describes a breaking change.
- Expose means to convert `str` into typed identifier with validation.

### Fixes

<!-- next-url -->
[Unreleased]: https://github.com/crate-ci/git-conventional/compare/v0.10.2...HEAD
[0.10.2]: https://github.com/crate-ci/git-conventional/compare/v0.10.1...v0.10.2
[0.10.1]: https://github.com/crate-ci/git-conventional/compare/v0.10.0...v0.10.1
[0.10.0]: https://github.com/crate-ci/git-conventional/compare/v0.9.2...v0.10.0
[0.9.2]: https://github.com/crate-ci/git-conventional/compare/v0.9.1...v0.9.2
[0.9.1]: https://github.com/crate-ci/git-conventional/compare/v0.9.0...v0.9.1
[0.9.0]: https://github.com/crate-ci/git-conventional/compare/v0.8.0...v0.9.0
[0.8.0]: https://github.com/crate-ci/git-conventional/compare/v0.7.0...v0.8.0
[0.7.0]: https://github.com/crate-ci/git-conventional/compare/ccaed9b35854a3536c4a2c89b89e33fbc5b6b4e4...v0.7.0
