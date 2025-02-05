# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [3.0.0] - 2019-11-08
- Add specific return types to all methods (previously `Promise<any>`)

## [2.3.0] - 2019-07-08
- Support `exemption_type` param for order-level exemptions
- Support `provider` param for marketplace exempt transactions
- Add types for nested objects (e.g., `line_items`)
- Refactor from Bluebird promises to native promises

## [2.2.2] - 2019-03-12
- Ignore `.DS_Store` when publishing to NPM

## [2.2.1] - 2019-03-12
- Correctly mark `exempt_regions` as optional in create/update customer methods

## [2.2.0] - 2018-11-01
- Support address validation for Plus customers via `validateAddress` method

## [2.1.2] - 2018-05-04
- Update dependencies

## [2.1.1] - 2018-05-03
- Convert each method from synchronous to asynchronous by returning a `Promise`
- Correctly mark `params` as optional in `ratesForLocation` and `list*` methods

## [2.1.0] - 2018-05-03
- Support customer exemptions

## [2.0.1] - 2018-03-22
- Send data in request body for POST and PUT requests

## [2.0.0] - 2018-03-21
- Require Node.js v4+ for Request dependency
- Sandbox environment support with `apiUrl` and custom headers
- Add further type definitions

## [1.4.1] - 2016-12-07
- Refactor away from deprecated `Promise.defer()` and improve error handling

## [1.4.0] - 2016-11-08
- Properly reject promise when API returns an error

## [1.3.0] - 2016-09-20
- Support `v2/nexus/regions` endpoint with new `nexusRegions` method
- Send data in query params for GET requests

## [1.2.0] - 2016-03-04
- Support VAT validation with new `validate` method
- Add new `summaryRates` method for calls to `v2/summary_rates`

## [1.1.2] - 2016-01-27
- Send all data to API as JSON

## [1.1.1] - 2015-08-18
- Default to `content-type` `application/json` for all requests

## [1.1.0] - 2015-07-23
- Add new methods to support listing, showing, and deleting transactions
- Drop `transactionId` param from `updateOrder` and `updateRefund`

## [1.0.2] - 2015-07-22
- `updateOrder` and `updateRefund` now send a PUT request to API

## [1.0.1] - 2015-07-22
- Set `content-type` to `application/json` for methods that send line items

## [1.0.0] - 2015-07-22
- Initial release

[Unreleased]: https://github.com/taxjar/taxjar-node/compare/v3.0.0...HEAD
[3.0.0]: https://github.com/taxjar/taxjar-node/compare/v2.3.0...v3.0.0
[2.3.0]: https://github.com/taxjar/taxjar-node/compare/v2.2.2...v2.3.0
[2.2.2]: https://github.com/taxjar/taxjar-node/compare/v2.2.1...v2.2.2
[2.2.1]: https://github.com/taxjar/taxjar-node/compare/v2.2.0...v2.2.1
[2.2.0]: https://github.com/taxjar/taxjar-node/compare/v2.1.2...v2.2.0
[2.1.2]: https://github.com/taxjar/taxjar-node/compare/v2.1.1...v2.1.2
[2.1.1]: https://github.com/taxjar/taxjar-node/compare/v2.1.0...v2.1.1
[2.1.0]: https://github.com/taxjar/taxjar-node/compare/v2.0.1...v2.1.0
[2.0.1]: https://github.com/taxjar/taxjar-node/compare/v2.0.0...v2.0.1
[2.0.0]: https://github.com/taxjar/taxjar-node/compare/v1.4.1...v2.0.0
[1.4.1]: https://github.com/taxjar/taxjar-node/compare/v1.4.0...v1.4.1
[1.4.0]: https://github.com/taxjar/taxjar-node/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/taxjar/taxjar-node/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/taxjar/taxjar-node/compare/v1.1.2...v1.2.0
[1.1.2]: https://github.com/taxjar/taxjar-node/compare/v1.1.1...v1.1.2
[1.1.1]: https://github.com/taxjar/taxjar-node/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/taxjar/taxjar-node/compare/v1.0.2...v1.1.0
[1.0.2]: https://github.com/taxjar/taxjar-node/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/taxjar/taxjar-node/compare/v1.0.0...v1.0.1
