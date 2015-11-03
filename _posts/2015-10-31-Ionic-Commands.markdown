---
layout: post
title:  "Ionic"
date:   2015-10-31 00:17:07 +0100
categories: Ionic
---

#### Usefull links
[Getting Started with Ionic](http://ionicframework.com/getting-started/)

[Ionic Documentation](http://ionicframework.com/getting-started/)

[AngularJS](https://angularjs.org/)

[AngularJS API Reference](https://docs.angularjs.org/api)

#### Install ionic and helfull dependencies
{% highlight bash %}
$ npm install -g cordova ionic eslint jshint gulp tsd
# In order to use sass.
$ ionic setup sass
# To get syntax recognision by the Visual Studio Code editor.
tsd query ionic angular --action install --save
{% endhighlight %}
#### Use ionic view to beta test your app
{% highlight bash %}
# Upload to ionic view. 
$ ionic upload --note "Fixed some bugs."
{% endhighlight %}

#### How to update the current ionic version in your project folder
{% highlight bash %}
$ ionic lib update
{% endhighlight %}

#### Generate icons and splash images
The folder "Resources" must exist and contain at least icon.png and splash.png.
{% highlight bash %}
# icon.png and splash.png is then used by the command.
$ icons resources
{% endhighlight %}

#### Run the local server
{% highlight bash %}
$ ionic serve
{% endhighlight %}

#### Build and run on android.
{% highlight bash %}
# Build tha android apk.
$ ionic build android
# Builds and runs the android apk on the attached device.
# Updates the javascript every time changes accures on the device
# and print the console messages out on the terminal.
$ ionic run android --livereload --consolelogs
{% endhighlight %}
