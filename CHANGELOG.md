## Release 0.2.2

### Bug fixes

- **Read key data from file passed to `key` parameter**
  ([#8](https://github.com/puppetlabs/puppetlabs-http_request/pull/8))

  Key data is now read from the file path passed to the `key` parameter.
  Previously, the file path itself was used as the key data.

## Release 0.2.1

### Bug fixes

- **Convert headers to strings**
  ([#4](https://github.com/puppetlabs/puppetlabs-http_request/pull/4))

  Headers set under the `headers` parameter are now converted to strings before
  making a request. Previously, headers were passed to the request as symbols.

  _Contributed by [barskern](https://github.com/barskern)._

## Release 0.2.0

### New features

- **Add `json_endpoint` parameter to `http_request` task**
  ([#2](https://github.com/puppetlabs/puppetlabs-http_request/issues/2))

  The `http_request` task now accepts a `json_endpoint` parameter. When set to
  `true`, the task will convert the request body to JSON, set the `Content-Type`
  header to `application/json`, and parse the response body as JSON.

## Release 0.1.0

This is the initial release.
