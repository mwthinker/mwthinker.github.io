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
