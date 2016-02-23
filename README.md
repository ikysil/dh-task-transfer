NOTE: I own the copyright on the source code and reserve the rights
to use it for whatever purpose I see fit, including publishing and
commercial use.

Total time spent: 9H 30M

# Implementation notes
## Assumptions

* curl tool is available in PATH
* "when it happened" from specification is the same as "when the task finished execution"
* command templates consists of tokens separated by one or more spaces, ($HOST) token is placeholder for host name
* no coordination is required when reporting results from different probes ("the data should contain 4 parts..."),
  "should" is interpreted as per [RFC-2119](https://www.ietf.org/rfc/rfc2119.txt)
* no explicit support for HTTP/HTTPS proxies is required
* no redirects processing is required
* no explicit support for custom HTTPS certificate chains is required
* no HA requirements
* no per-host configuration is required except for host name

## TODO
* Validation of the configuration parameters
* Unit tests are almost missing

