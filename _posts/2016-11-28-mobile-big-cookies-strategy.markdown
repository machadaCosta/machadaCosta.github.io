---
layout: post
title:  "Big Cookies Strategy"
date:   2016-11-28
author: Macha Da Costa
category: mobile
tags: [mobile development, big cookies strategy]
excerpt: This post is about the Big Cookies Strategy for exchange between server and mobile.
permalink: /mobile-big-coukies-strategy/
---

Big Cookies Strategy was created to optimize exchange between a mobile application and a server.
 

## What is Big Cookies Strategy ?

![Big Cookies Strategy in Mobile Development]({{ site.baseurl }}/img/big-cookies-strategy.png)


<i class="fa fa-list" aria-hiden="true"></i> Step by step : 
1. Verify that connection is available on mobile
2. Ask needed data to server with the connectivity state in user agent
3. Receive prefetched* data from server

* Belonging to the mobile connectivity state, server send data set of different size

For instance, 
Connectivity | Data set 
-------------|:---------:
Edge | Info since one or two hour
3G or 4G | Info since 3 days
Wifi | Info since 15 days 



