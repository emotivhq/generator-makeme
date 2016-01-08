## Generators

Here are the currently included generators:

* App
    - [makeme](#app) (aka [makeme:app](#app))
* Server Side
    - [makeme:endpoint](#endpoint)
* Client Side
    - [makeme:route](#route)
    - [makeme:controller](#controller)
    - [makeme:filter](#filter)
    - [makeme:directive](#directive)
    - [makeme:service](#service)
    - [makeme:provider](#service)
    - [makeme:factory](#service)
    - [makeme:decorator](#decorator)
* Deployment
    - [makeme:openshift](#openshift)
    - [makeme:heroku](#heroku)

## App
Sets up a new AngularJS + Express app, generating all the boilerplate we need.

Usage:
```bash
Usage:
  yo makeme:app [options] [<name>]

Options:
  -h,   --help          # Print the generator's options and usage
        --gulp          # Use the Gulp config instead of Grunt                  Default: false
        --skip-cache    # Do not remember prompt answers                        Default: false
        --skip-install  # Do not install dependencies                           Default: false
        --app-suffix    # Allow a custom suffix to be added to the module name  Default: App

Arguments:
  name    Type: String  Required: false
```

Example:
```bash
yo makeme --gulp new-app
```

## Endpoint
Generates a new API endpoint.

#### Usage:
```bash
Usage:
  yo makeme:endpoint [options] <name>

Options:
  -h,   --help               # Print the generator's options and usage
        --skip-cache         # Do not remember prompt answers           Default: false
        --route              # URL for the endpoint
        --models             # Specify which model(s) to use
        --endpointDirectory  # Parent directory for enpoints

Arguments:
  name    Type: String  Required: true
```

#### Example:
```bash
yo makeme:endpoint message
[?] What will the url of your endpoint be? /api/messages
```

#### Produces:

    server/api/message/index.js
    server/api/message/index.spec.js
    server/api/message/message.controller.js
    server/api/message/message.integration.js
    server/api/message/message.model.js  (optional)
    server/api/message/message.events.js (optional)
    server/api/message/message.socket.js (optional)

## Route
Generates a new module with built in route.

#### Example:
```bash
yo makeme:route mymodule
[?] Where would you like to create this route? client/app/
[?] What will the url of your route be? /mymodule
```

#### Produces:

    client/app/mymodule/mymodule.js
    client/app/mymodule/mymodule.controller.js
    client/app/mymodule/mymodule.controller.spec.js
    client/app/mymodule/mymodule.html
    client/app/mymodule/mymodule.scss


## Controller
Generates a controller.

#### Example:
```bash
yo makeme:controller user
[?] Where would you like to create this controller? client/app/
```

#### Produces:

    client/app/user/user.controller.js
    client/app/user/user.controller.spec.js

## Directive
Generates a directive.

#### Example:
```bash
yo makeme:directive myDirective
[?] Where would you like to create this directive? client/app/
[?] Does this directive need an external html file? Yes
```

#### Produces:

    client/app/myDirective/myDirective.directive.js
    client/app/myDirective/myDirective.directive.spec.js
    client/app/myDirective/myDirective.html
    client/app/myDirective/myDirective.scss

### Simple directive without an html file

#### Example:
```bash
yo makeme:directive simple
[?] Where would you like to create this directive? client/app/
[?] Does this directive need an external html file? No
```

#### Produces:

    client/app/simple/simple.directive.js
    client/app/simple/simple.directive.spec.js

## Filter
Generates a filter.

#### Example:
```bash
yo makeme:filter myFilter
[?] Where would you like to create this filter? client/app/
```

#### Produces:

    client/app/myFilter/myFilter.filter.js
    client/app/myFilter/myFilter.filter.spec.js

## Service
Generates an AngularJS service.

#### Example:
```bash
yo makeme:service myService
[?] Where would you like to create this service? client/app/
```

#### Produces:

    client/app/myService/myService.service.js
    client/app/myService/myService.service.spec.js


You can also do `yo makeme:factory` and `yo makeme:provider` for other types of services.

## Decorator
Generates an AngularJS service decorator.

####Example:
```bash
yo makeme:decorator serviceName
[?] Where would you like to create this decorator? client/app/
```

####Produces

    client/app/serviceName/serviceName.decorator.js