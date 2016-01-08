## Gulp tasks
Main gulp tasks:

```
gulp build          # Build the app
gulp serve          # Load the app in preview mode
gulp serve:debug	# Load a more debugging-friendly environment
gulp dist           # Distribute the application
```

All build tasks

```
gulp build:images   # Just build images
gulp copy:extras	# copy extras to dist
gulp copy:assets    # copy assets to dist
gulp copy:server    # copy server files
```
All test tasks
```
gulp test:e2e               # runs end2end tests with Selenium webdriver
gulp mocha:coverage         # runs full test coverage with Mocha (unit, integration, env, coverage)
gulp coverage:integration   # run integration tests
gulp coverage:unit          # run unit tests
gulp coverage:pre           # run pre tests
```

Detailed gulp tasks

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

Start the client & server 
```
gulp start:server   # start the Node/Express server
gulp start:client   # start the local app up (no server)
gulp watch          # the watch `command`
```
Set ENV variables
```
gulp env:all        # set local dev environment
gulp env:test       # set the local ENV variable to `test`
gulp env:prod       # set the local ENV variable to `prod`
```
