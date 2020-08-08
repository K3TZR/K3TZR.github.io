---
layout: post
title:  "Using xLib6000 to connect to your Radio"
date:   2020-08-07 20:00:00 -0400
categories: jekyll update
---
A number of you have asked "How do I use xLib6000"? Unfortunately, there isn't a nice manual on that topic. At least so far, my time is better spent fixing bugs and implementing missing features.

Instead of a manual I've prepared an example. It turns out that a Non-Gui connection just isn't that difficult. The example is called:

    xLibSimpleExample

You can find the sorce code at [xLibSimpleExample](https://github.com/K3TZR/xLibSimpleExample)  
For an executable version look at the [Current Release](https://github.com/K3TZR/xLibSimpleExample/releases/tag/v1.0.1) page.

The app works with both the old, API radios ( version < 2.6) as well as the new API (version >= 2.6). The principal difference being that in the old API you did not have to "bind" to a "station".

It's written using SwiftUI (I needed the practice) but all of the code that demonstrates how to connect can be found in the RadioManager.swift file. Look at the ***Connect*** and the ***Disconnect*** methods. If you are using a New API radio, you also need to look at the ***Bind*** and the ***Unbind*** methods.

There are instructions for using the app in the README.md file as well as in the source code. I've made an attempt to make the code as simple as possible. I've also commented almost every line.

Let me know if it was helpful.

73's Doug, K3TZR
