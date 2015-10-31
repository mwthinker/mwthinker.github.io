---
layout: post
title:  "Sencha Touch 2"
date:   2015-10-31 00:17:07 +0100
categories: Sencha Touch 2
---

#### Usefull links
[Touch Guides](http://docs.sencha.com/touch/2.4/)
[Touch Sencha Docs](http://docs.sencha.com/touch/2.4/2.4.2-apidocs/)

#### Create a new Sencha project
{% highlight bash %}
$ cd C:\sencha\touch-2.4.2
$ sencha generate app -name ExampleProject -path C:\Projects
{% endhighlight %}

#### Start a local web-server
{% highlight bash %}
$ sencha fs web -p 80 start -map C:\Projects
{% endhighlight %}

#### Automatic compilation of the app
{% highlight bash %}
$ cd C:\Projects\ExampleProject
$ sencha app watch
{% endhighlight %}

#### Build and/or run the native app.
{% highlight bash %}
$ cd C:\Projects\ExampleProject
$ sencha app build native

$ cd C:\Projects\ExampleProject
$ sencha app run native
{% endhighlight %}

#### Sometimes files are missing in the compiled project (chrome)
{% highlight bash %}
$ cd C:\Projects\ExampleProject
$ sencha app refresh
{% endhighlight %}

#### Update the touch 2 version for the app
{% highlight bash %}
$ cd C:\Projects\ExampleProject
$ sencha app upgrade <Path to Sencha Touch 2.4 SDK>
{% endhighlight %}
