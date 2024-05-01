# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres
to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Fixed

* Test query parameters (`params`) may have been passed with trailing data from the test suite because scalars were
  processed without their length. This could have led to sending superfluous trailing data to Postgres.

## [0.3.0]

### Added

* Test suites (YAML files) can now be named using optional `name` property.
* Tests can now reset connections with the boolean `reset` property.
* Tests can now be executed without a transaction (for non-transactional commands) using optional `transaction` property
* Tests can now be executed on a different database using optional `database` property
* Default encoding and locale for databases can be specified using `encoding` and `locale` property of `instance`

## [0.2.0]

### Added

* Support for unmanaged (external) instances

## [0.1.0] - 2023-08-25

Initial release following a few months of iterative development.

[Unreleased]: https://github.com/omnigres/omnigres/commits/master/pg_yregress

[0.3.0]: https://github.com/omnigres/omnigres/releases/tag/pg_yregress/v0.3.0

[0.2.0]: https://github.com/omnigres/omnigres/releases/tag/pg_yregress/v0.2.0

[0.1.0]: https://github.com/omnigres/omnigres/releases/tag/pg_yregress/v0.1.0
