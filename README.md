# DrivingScout NodeJS SDK

Enables you to find [driving test cancellations](https://drivingscout.uk) via [DrivingScout](https://drivingscout.uk).

## Installation
```sh
$ npm install drivingscout
```

## Usage
There is currently only one function, `register`, which is used to initiate the registration with DrivingScout. This requires a pre-pay billing account, please reach out to us via hello@drivingscout.uk to understand more.

```javascript
drivingscout.register(params, callback);

```

`params` will depend on your setup with us, and will be listed in your welcome email.


Example code:

```javascript
var drivingscout = require('drivingscout');

drivingscout.register(params, function callback(err, msg) {
  if (err) {
    console.error(err);
  } else {
    // Success! Registration with DrivingScout complete.
  }
});

```
