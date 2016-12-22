# Sunrise Java Starter Project
[![Build Status](https://travis-ci.org/commercetools/commercetools-sunrise-java-starter.svg?branch=master)](https://travis-ci.org/commercetools/commercetools-sunrise-java-starter)

Sunrise-based project using:
- [Sunrise Shop Framework](https://github.com/commercetools/commercetools-sunrise-java)
- [Sunrise Theme](https://github.com/commercetools/commercetools-sunrise-theme)
- [Play Web Framework 2.5.x](https://www.playframework.com/documentation/2.5.x/Home)

Use it as the starting point to develop your own online shop project.

## Preconditions

* Install [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (version >= 1.8.0_92)
* Create a [commercetools platform project](https://admin.sphere.io/en/signup) with some data
* Unless you modify the project to behave differently:
  * Product variants must contain a SKU without dashes `-`

## Run it locally

First, put the credentials of your commercetools platform project in `conf/dev.conf` as follows:

```properties
ctp.projectKey = your-project-key
ctp.clientId = your-client-id
ctp.clientSecret = your-client-secret
ctp.authUrl = "https://auth.sphere.io"
ctp.apiUrl = "https://api.sphere.io"
```

If you have [SBT](http://www.scala-sbt.org/) on your computer you can run it with `sbt ~run`. Otherwise you can use the [Activator](https://www.lightbend.com/community/core-tools/activator-and-sbt) found in the project to run it locally:

* on Linux/Mac: `./activator ~run` 
* on Windows: `activator ~run`

In any case, the output will be similar to:

```
[info] play - Listening for HTTP on /0:0:0:0:0:0:0:0:9000
(Server started, use Ctrl+D to stop and go back to the console...)
```

Now open <a href="http://localhost:9000">http://localhost:9000</a> in your browser and you should be able to access the web application using your project.

## Deployment

For an easy and fast deployment of your application we recommend [Heroku](https://www.heroku.com):

<a href="https://heroku.com/deploy?template=https://github.com/commercetools/commercetools-sunrise-java-starter/tree/master"><img src="https://www.herokucdn.com/deploy/button.png" alt="Deploy"></a>
