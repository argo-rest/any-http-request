# AnyHTTP adapter for Node (request)

[AnyHTTP](https://github.com/argo-rest/any-http) adapter for the
Node [request](https://www.npmjs.com/package/request) HTTP library.

## Usage

This adapter is implemented as an ES6 module which can be installed
with [jspm](https://jspm.io) and loaded via
[SystemJS](https://github.com/systemjs/systemjs) as follows:

``` javascript
import {Http} from 'github:argo-rest/any-http-request;

var httpClient = new Http;
httpClient.
  get('https://example.com').
  then(({body, headers}) => {
    console.log("body:", body);
    console.log("content-type:", headers['Content-Type']);
  });
```
