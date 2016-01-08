## Gulp tasks
Main gulp tasks:

```
gulp serve          # Load the application in preview mode
gulp test           # Test the application
gulp build          # Build the application
```

All serve tasks.

```
gulp serve          # Load the application in preview mode
gulp serve:debug	# Load a more debugging-friendly environment
gulp serve:dist	    # Load from the built application in dist
```

All test tasks.

```
gulp test                   # runs all tests everywhere, in the world
gulp test:e2e               # runs end2end tests with Selenium webdriver
gulp mocha:coverage         # runs full test coverage with Mocha (unit, integration, env, coverage)
gulp coverage:integration   # run integration tests
gulp coverage:unit          # run unit tests
gulp coverage:pre           # run pre tests
```

All build & distribute tasks.

```
gulp build          # Build & distribute the application
gulp build:images   # Just build images
gulp copy:extras	# Copy the extras to dist
gulp copy:assets    # Copy the assets to dist
gulp copy:server    # Copy the server files
```

Detailed gulp tasks.

```
gulp help           # List the main gulp tasks
gulp lint:scripts   # Run lint
gulp inject         # inject js, css, and scss (you can also run `gulp inject:scss`)
gulp wiredep:client # inject bower and other local components
gulp test           # Run lint, unit tests, and e2e tests
gulp unit           # Run lint and unit tests (karma for client + mocha for server)
gulp karma          # Run karma client unit tests
gulp mocha          # Run mocha server unit tests
gulp e2e            # Run protractor for end to end tests
gulp styles         # Generate a main app.css file
gulp constant       # Build and inject constants
```

Start the client & server.

```
gulp start:server   # start the Node/Express server
gulp start:client   # start the local app up (no server)
gulp watch          # the watch `command`
```

Set ENV variables.

```
gulp env:all        # set local dev environment
gulp env:test       # set the local ENV variable to `test`
gulp env:prod       # set the local ENV variable to `prod`
```
