## Testing

Running `gulp test` will run the client and server unit tests with karma and mocha.

To only run server tests.

```
gulp test:server
```

To only run client tests.

```
gulp test:client
```

### Protractor tests

To setup protractor end to end (`e2e`) tests, first run...

```
npm run update-webdriver`
```

Then, to have protractor go through tests located in the `e2e` folder...

```
grunt test:e2e
```

### Code Coverage

To run `mocha-istanbul` and generate `code coverage` reports...

```
grunt test:coverage
```

> `coverage/server` will be populated with `e2e` and `unit` folders containing the `lcov` reports.

The coverage taget has 3 available options:

- `test:coverage:unit` generate server unit test coverage
- `test:coverage:e2e` generate server e2e test coverage
- `test:coverage:check` combine the coverage reports and check against predefined thresholds

> *When no option is given `test:coverage` runs all options in the above order*

### Debugging

For a more debugging-friendly environment...

```
grunt serve:debug
```