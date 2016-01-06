## Deployment & build control
One command hot deployments. 

### Heroku

Deploying to heroku only takes a few steps.

To create a new Heroku app...
```
yo makeme:heroku
```

> **Important:** To work with the new heroku app using the command line, you will need to run any `heroku` commands from the `dist` folder.


If you're using mongoDB you will need to add a database to your app:

```
heroku addons:create mongolab
```

#### Your app should now be live. To view it run `heroku open`.

---

> If you're using any oAuth strategies, you must set environment variables for your selected oAuth. For example, if we're using **Facebook** oAuth we would do this :
>
>     heroku config:set FACEBOOK_ID=id
>     heroku config:set FACEBOOK_SECRET=secret
>
> You will also need to set `DOMAIN` environment variable:
>
>     heroku config:set DOMAIN=<your-heroku-app-name>.herokuapp.com
>
>     # or (if you're using it):
>
>     heroku config:set DOMAIN=<your-custom-domain>
>

To make your deployment process easier consider using [grunt-build-control](https://github.com/robwierzbowski/grunt-build-control).

#### Pushing Updates

```
gulp
```

Commit and push the resulting build, located in your `dist` folder:

``` 
gulp buildcontrol:heroku
```



### Openshift

Deploying to OpenShift can be done in just a few steps:

    yo makeme:openshift

A live application URL will be available in the output.

> **oAuth**
>
> If you're using any oAuth strategies, you must set environment variables for your selected oAuth. For example, if we're using Facebook oAuth we would do this :
>
>     rhc set-env FACEBOOK_ID=id -a my-openshift-app
>     rhc set-env FACEBOOK_SECRET=secret -a my-openshift-app
>
> You will also need to set `DOMAIN` environment variable:
>
>     rhc set-env DOMAIN=<your-openshift-app-name>.rhcloud.com
>
>     # or (if you're using it):
>
>     rhc set-env DOMAIN=<your-custom-domain>
>
> After you've set the required environment variables, restart the server:
>
>     rhc app-restart -a my-openshift-app

To make your deployment process easier consider using [grunt-build-control](https://github.com/robwierzbowski/grunt-build-control).

#### Pushing Updates

```
gulp
```

Commit and push the resulting build, located in your `dist` folder:

```
gulp buildcontrol:openshift
```