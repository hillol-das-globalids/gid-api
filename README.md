# \<gid-api\>

The `gid-api` element is a wrapper on iron ajax used for handling rest calls.

    <gid-api auto=false
			http-method="get" api-url="../assets/json/test.json" response={{ajaxResponse}}
			api-timeout= 0  api-params='{"token": "AIzaSyAuecFZ9xJXbGDkQYWBmYrtzOGJD-iDIgI"}'>
    </gid-api>

With `auto` set to `true`, the element performs a request whenever its `url`, `params` or `body` properties are changed. Automatically generated requests will be debounced in the case that multiple attributes are changed sequentially.
The `params` attribute must be double quoted JSON.

You can trigger a request explicitly by calling `generateRequest` on the element.


## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.