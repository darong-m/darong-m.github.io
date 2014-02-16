---
layout: post
title: "Failed to build gem native extension"
date: 2014-02-16 18:03:19 +0700
comments: true
categories:
---

Steps involved

- Download and install 7-zip.
- Download the Development Kit and install it in say c:\devkit.
- Open a command window and type c:.
- Change folders by typing cd devkit.
- Type ruby dk.rb init to generate the config.yml file to be used later. Your installed Rubies will be listed there (only those installed by a RubyInstaller package are detected at present). This needs to be done only once.
- Finally type, ruby dk.rb install for DevKit enhance your installed Rubies. This needs to be done only once.
- Confirm your Ruby environment is correctly using the DevKit by running: gem install bson_ext --platform=ruby. It’s crucial that you include the --platform=ruby option to force RubyGems to build the native gem rather than potentially installing an incorrect binary gem.

Fore more information, see [here](http://rubylearning.com/blog/how-do-i-install-a-ruby-gem-with-native-extensions-on-windows/).
