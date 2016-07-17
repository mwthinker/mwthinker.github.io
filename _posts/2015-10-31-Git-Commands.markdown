---
layout: post
title:  "Git"
date:   2015-10-31 00:17:07 +0100
categories: Git
---

#### Git branch replace
[Replacing one git branch with another one](http://code.opoki.com/replacing-one-git-branch-with-another-one/)
{% highlight bash %}
$ git checkout new_master
# merge master - ignoring master's changes
$ git merge -s ours master
$ git checkout master
# finally merge all our stuff to new master - actually it replaces the master with new_master
$ git merge new_master
# now new_master can be deleted
{% endhighlight %}

#### How to ignore filees already added/initialized in repository
{% highlight bash %}
$ git rm --cached myFileName
$ git add .
$ git commit -m ".gitignore is now working"
{% endhighlight %}

#### Submodules
Update to the latest version of your submodules.
{% highlight bash %}
$ git submodule foreach git pull origin master
{% endhighlight %}

Download all current submodules and initilize them.
{% highlight bash %}
$ git submodule update --init --recursive
{% endhighlight %}

Add a submodule.
{% highlight bash %}
$ git submodule add https://github.com/mwthinker/MwLibrary2.git
{% endhighlight %}

Remove a submodule.
{% highlight bash %}
$ git submodule deinit MwLibrary2
$ git rm MwLibrary2
{% endhighlight %}

Note: MwLibrary2 (no trailing slash)
or, if you want to leave it in your working tree.
{% highlight bash %}
git rm --cached MwLibrary2
{% endhighlight %}

#### Tags
[Tags on github](https://help.github.com/articles/working-with-tags/)

Add a tag.
{% highlight bash %}
$ git tag -a v0.7 -m 'Playable using Open GL ES 2, but must be polished'
$ git tag -a v2.0.1 -m 'Only SDL libraries and OpenGL dependencies'
{% endhighlight %}

To make them show up on github.
{% highlight bash %}
$ git push --tags master
{% endhighlight %}
