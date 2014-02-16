---
layout: post
title: "Getting started with Octopress"
date: 2014-02-16 16:02:12 +0700
comments: true
categories: octopress
---

This blog has been setup many months ago, but I don't have time to update it. Today I decide to update it. Unfortunately, I run into a problem with run *rake deploy*. It always reject the request to push to master branch.
I've setup the octopress for many times today. Issues still exist:

- How to change git url for the blog
- Make codeblock work when setting language

It may be because I am not familiar with Octopress itself. Hope to find a solution soon.

- At last, I find a guide to setup octopress in Windows. [Link](http://blog.zerosharp.com/setting-up-octopress-on-windows-again/) here. In the same time, it also describes how to solve issue with codeblock.

- Gem::RemoteFetcher::FetchError: SSL_connect returned=1 errno=0 state=SSLv3 read server certificate B: certificate verify failed (https://rubygems.org/gems/rake-0.9.6.gem). [Link](https://gist.github.com/fnichol/867550) to solve this issue. It seems I have to add environment variable through control panel to fix this issue.
