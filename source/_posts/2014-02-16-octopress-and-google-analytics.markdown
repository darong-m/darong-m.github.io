---
layout: post
title: "Octopress and google analytics"
date: 2014-02-16 15:36:51 +0700
comments: true
categories: [octopress, google analytics]
---

When hosting octopress on github, just provide the google analytics track id is not enough.
I need to edit file *source/_includes/google_analytics.html* in the source tree. I add extra line of javascript to the default script.

{% codeblock lang:js %}
_gaq.push(['_setAccount', '{{ site.google_analytics_tracking_id }}']);
_gaq.push(['_setDomainName','github.io']);
_gaq.push(['_trackPageview']);
{% endcodeblock %}
