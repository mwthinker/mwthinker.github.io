---
layout: post
title:  "Cordova"
date:   2015-10-31 00:17:07 +0100
categories: Cordova
---

Nodejs must be installed and added to PATH in order for the commands to work.

#### Install Cordova
{% highlight bash %}
$ npm install -g cordova
{% endhighlight %}

#### Update to latest Cordova and the project (android)
{% highlight bash %}
$ npm update -g cordova
$ cordova platform update android
{% endhighlight %}

#### Add platform to Cordova project
{% highlight bash %}
$ cordova platform add android ios
{% endhighlight %}

#### Check the current platforms
{% highlight bash %}
$ cordova platforms ls
{% endhighlight %}

#### List all installed plugins
{% highlight bash %}
$ cordova plugin ls
{% endhighlight %}

#### Add/remove installed plugins
{% highlight bash %}
$ cordova plugin add org.apache.cordova.console
$ cordova plugin rm org.apache.cordova.console
{% endhighlight %}

#### Build the native app.
{% highlight bash %}
$ cordova build
{% endhighlight %}
